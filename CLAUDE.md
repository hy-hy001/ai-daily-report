# AI Daily Report

## 项目概览

每日自动生成 AI 日报（AIHOT 数据源），通过 GitHub Actions + Windows 定时任务实现全自动化流水线。

## 架构：Worktree Agent 流水线

```
main                          GitHub Actions (06:03 Beijing → 云端抓取 AIHOT → AI日报.md)
│
├── agent/sync                Sync agent (06:10 → 从 GitHub 拉到 Obsidian + 桌面)
├── agent/triage              Triage agent (07:00 → 三检: GA/Obsidian/Desktop)
├── agent/evaluator           Evaluator (07:00 triage 内联调用 → 5 道质量门禁)
└── agent/daily               Daily agent (备用手动抓取)
```

每个 agent 在独立 worktree 分支上运行，互不干扰。

## 关键文件

| 文件 | 位置 | 职责 |
|------|------|------|
| `daily-report.yml` | `.github/workflows/` | GitHub Actions 云端抓取 AIHOT 并生成日报 |
| `ai_daily_sync.ps1` | `.worktrees/sync/` (agent/sync) | 从 GitHub 克隆 → 复制到 Obsidian + 桌面 |
| `aihot_triage.ps1` | `.worktrees/triage/` (agent/triage) | 三检: GitHub Actions 状态 / Obsidian 日期 / 桌面一致性 |
| `aihot_evaluator.ps1` | `.worktrees/evaluator/` (agent/evaluator) | 5 道门禁: 状态文件/AI日报/代码规范/Workflow/外部依赖 |
| `aihot_daily.ps1` | `.worktrees/daily/` (agent/daily) | 本地备用手动抓取脚本 |
| `AI日报.md` | Obsidian 仓库 + 桌面 | 生成的日报内容 |
| `AI日报-运行状态.md` | Obsidian 仓库 + 桌面 | 三检 + 评估报告追踪 |

## 定时任务

| 时间 (北京) | 任务 | 脚本路径 |
|-------------|------|----------|
| 06:03 | GitHub Actions (云端) | `.github/workflows/daily-report.yml` |
| 06:10 | AI日报同步 (Windows) | `.worktrees/sync/ai_daily_sync.ps1` |
| 07:00 | AI日报三检 (Windows) | `.worktrees/triage/aihot_triage.ps1` 内联调用 evaluator |

Windows 定时任务配置了 10 分钟超时自动终止。

## 开发指南

### 修改 agent 脚本

```bash
# 先 cd 到对应 worktree
cd .worktrees/triage
# ... 修改 ...
git commit -am "fix: ..."
git push origin agent/triage
```

### 手动触发一次流水线

```powershell
# 手动跑一次 GitHub Actions
# GitHub → Actions → AI 日报精选 TOP 10 → Run workflow

# 手动同步
.\.worktrees\sync\ai_daily_sync.ps1

# 手动检查
.\.worktrees\triage\aihot_triage.ps1
```

## 环境依赖

- PowerShell 7+（Windows 定时任务）
- Git（worktree 管理）
- GitHub Token（git push 用 token-embedded URL 绕过代理）
- 网络：AIHOT API / GitHub API 可达
