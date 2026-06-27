# 🤖 AI 日报精选 TOP 10

每日自动抓取 [AIHOT](https://aihot.virxact.com) 精选评分，生成 TOP 10 日报。

## 流水线架构

```
06:03  GitHub Actions (云端) → 抓取 AIHOT → 提交 AI日报.md 到仓库
                  ↓
06:10  Sync agent (Windows) → 克隆仓库 → 复制到 Obsidian 仓库 + 桌面
                  ↓
07:00  Triage agent (Windows) → 三检：GA 状态 / Obsidian 日期 / 桌面一致性
                  ↓
        Evaluator (Windows) → 5 道质量门禁 → 追加评估报告到状态文件
```

每个 agent 在 [独立 git worktree](CLAUDE.md) 上运行，互不干扰。

## 关键文件

| 文件 | 位置 | 说明 |
|------|------|------|
| `AI日报.md` | 仓库根目录 / Obsidian 仓库 / 桌面 | 每日生成的日报 |
| `AI日报-运行状态.md` | Obsidian 仓库 / 桌面 | 三检 + 评估追踪 |

## 本地使用

```powershell
# 手动拉取最新日报到本地
.\.worktrees\sync\ai_daily_sync.ps1

# 手动运行三检 + 评估
.\.worktrees\triage\aihot_triage.ps1

# 手动抓取 AIHOT（备用）
.\.worktrees\daily\aihot_daily.ps1
```

## Obsidian 同步

安装 [Obsidian Git](https://github.com/denolehov/obsidian-git) 插件，将本仓库 clone 到 Obsidian 仓库目录下即可自动接收每日更新。

## 更新频率

每天北京时间 **06:03** GitHub Actions 自动更新。
