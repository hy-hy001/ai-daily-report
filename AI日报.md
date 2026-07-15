# AI 日报精选 TOP 10
**2026-07-16** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. xAI 官方 Grok CLI 被曝静默上传整个代码库及用户密钥
🔴 评分 **86** · 公众号：数字生命卡兹克 · 2 天前

> 安全研究者发现，xAI 官方 Grok CLI（npm 包 `@xai-official/grok` 0.2.93 版）会在每轮任务前后，将当前工作目录打包为 `before_codebase.tar.gz` 和 `after_codebase.tar.gz`，通过独立旁路通道静默上传至 xAI 的 Google Cloud 仓库。验证显示，即使模型仅回复一个单词，上传依然发生。上传包还包含仓库外的 `~/.claude.json`、Claude Code 设置、全局 AGENTS 规则、30 多个 Skill 文件及一个 API 密钥。7 月 13 日凌晨，xAI 通过服务端远程开关新增 `disable_codebase_upload` 字段，将默认上传行为关闭，但此前该功能默认开启。

🔗 [阅读原文](https://mp.weixin.qq.com/s/6c6vGMJAVMbh6UhNVw4dcg)

---

### 2. Cursor IDE 0day 漏洞：打开恶意仓库即可自动执行任意代码
🔴 评分 **83** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> 安全公司 Mindgard 于 2025 年 12 月 15 日发现 Cursor IDE 存在严重 0day 漏洞。当用户在 Windows 上打开包含恶意 `git.exe` 的仓库时，Cursor 会自动执行该文件，无需任何用户交互。漏洞源于 Cursor 在加载项目时会在包括工作区在内的多个位置搜索 Git 二进制文件。Mindgard 在 7 个月内多次报告，Cursor CISO 虽确认但因内部自动化故障导致流程中断，至今已发布 70 多个新版本仍未修复。临时缓解措施包括使用 AppLocker 阻止从工作区目录执行该文件名，或在隔离虚拟机中打开不受信任的仓库。

🔗 [阅读原文](https://mindgard.ai/blog/cursor-0day-when-full-disclosure-becomes-the-only-protection-left)

---

### 3. 国行 Apple 智能完成备案，阿里千问将集成至苹果 AI 能力
🔴 评分 **82** · IT之家（RSS） · 14 小时前

> 苹果技术开发（上海）有限公司的"Apple 智能"大模型已于 2026 年 7 月 8 日完成备案，适用场景为苹果手机。阿里千问将作为 AI 能力集成至 Apple 智能，为 iOS、iPadOS、macOS 和 visionOS 的中国用户提供文本与图像理解、内容生成等功能，用户无需在应用间切换即可直接体验。

🔗 [阅读原文](https://www.ithome.com/0/977/109.htm)

---

### 4. 阿里Qwen将集成至Apple Intelligence服务中国用户
🟠 评分 **78** · X：X.PIN (@thexpin) · 12 小时前

> 阿里巴巴的Qwen模型将被集成到Apple Intelligence中，为中国的iOS、iPadOS、macOS和visionOS用户提供文本与图像理解、内容生成等AI功能。中国网信办已公布包括Apple Intelligence、华为小艺大模型、OPPO AndesGPT在内的七项移动端生成式AI服务备案信息。阿里巴巴董事会主席蔡崇信表示，苹果在选定阿里前曾与多家中国公司洽谈。

🔗 [阅读原文](https://x.com/thexpin/status/2077346752219521469)

---

### 5. Airtap iMessage 新功能：发条短信让 AI 替你操作手机
🟠 评分 **78** · X：阿易 AI Notes (@AYi_AInotes) · 20 小时前

> Airtap 推出 iMessage 新功能，用户只需给美国号码发一条 iMessage，其云手机上的 AI Agent 就能通过视觉模拟点击，替用户完成 TikTok 刷视频、星巴克点单等操作，无需安装对应 App。其架构分为三层：大脑（理解指令）、AutoPilot（视觉操控屏幕）、云手机（24小时在线）。但支付等敏感操作仍需用户手动完成，信任与授权仍是所有 Agent 厂商的难题。

🔗 [阅读原文](https://x.com/AYi_AInotes/status/2077217295504490992)

---

### 6. OpenAI 面向普通用户发布提示词指南：从结果出发，少写步骤
🟠 评分 **78** · The Decoder：AI News（RSS） · 2 天前

> OpenAI 整合了一份面向普通用户的提示词指南，涵盖目标、上下文、输出格式和边界四个可选模块。指南建议以结果而非步骤开头，用一两条硬性规则替代逐步骤脚本。Chat 处理快速任务，基于 Codex 技术和 GPT-5.6 模型的 ChatGPT Work 负责多源、多步骤的复杂项目。Codex 新增 Steer（重定向当前运行）、Queue（排队下一条消息）和沙盒模式，支持 `/plan`、`/goal` 和 `/review` 等斜杠命令。用户无需一次性写对提示词，后续追问是预期调整方式。

🔗 [阅读原文](https://the-decoder.com/openais-new-prompting-guide-tells-users-to-stop-overthinking-and-start-with-the-result)

---

### 7. Telegram 无服务器架构
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 7 小时前

> Telegram Serverless 允许开发者直接在 Telegram 基础设施上运行 Bot 和 Mini App 的后端代码，无需配置服务器或容器。开发者编写普通 JavaScript 模块，通过 `npx tgcloud push` 单命令部署，代码在靠近 Bot API 和内建数据库的轻量级 V8 隔离沙箱中执行。

🔗 [阅读原文](https://core.telegram.org/bots/serverless)

---

### 8. 前沿模型实际成本：tokenizer 差异导致隐性涨价
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 2 天前

> 同一份 TypeScript 文件在 GPT-5.x 上为 681 个 token，在 Claude 最新 tokenizer 下为 1，178 个，相差 1.73 倍。Anthropic 新 tokenizer 比旧版多产生约 30% 的 token，标价不变，构成隐性涨价。Claude Opus 4.6 与 Opus 4.8 标价同为 $5.00 / $25.00，但新 tokenizer 使同一代码的 token 数增加约 32%。Claude Sonnet 5 的 $2.00 / $10.00 为促销价，2026 年 8 月 31 日后恢复 $3.00 / $15.00，届时相同代码成本将比 Sonnet 4.6 高出约 32%。跨厂商对比中，Claude 新 tokenizer 在代码上比 GPT 多产生 1.50x 至 1.73x 的 token，TypeScript 差距最大。

🔗 [阅读原文](https://playcode.io/blog/real-price-of-frontier-models)

---

### 9. Meta 宣布扩建路易斯安那州数据中心至 5GW，总投资超 500 亿美元
🟠 评分 **77** · IT之家（RSS） · 2 天前

> Meta 将其路易斯安那州数据中心算力扩至 5GW，总投资超 500 亿美元，为全球最大 AI 基础设施投资之一。Meta 承诺承担全部能源及水资源费用，并另投超 10 亿美元改善当地道路及供水系统。此外，Meta 与安特吉公司达成协议，为新建天然气发电厂、储能电池及核电增容项目提供资金支持。

🔗 [阅读原文](https://www.ithome.com/0/976/149.htm)

---

### 10. 黄仁勋：英伟达季度收入逼近千亿美元，Rubin Ultra 架构未延期
🟠 评分 **77** · IT之家（RSS） · 2 天前

> 英伟达CEO黄仁勋在摩根士丹利路演中表示，公司季度营收即将逼近1000亿美元，且增长速度仍在加快。他否认下一代旗舰架构Rubin Ultra延期传闻，称其仍按计划于明年出货，当前机架设计调整仅为系统架构优化。一个此前主要依赖ASIC的前沿AI模型项目，如今英伟达GPU算力占比已接近50%，市场普遍指向Anthropic。英伟达预计本财年CPU业务收入约200亿美元，下一代Vera CPU将进军通用服务器市场。摩根士丹利维持英伟达"增持"评级，目标价288美元。

🔗 [阅读原文](https://www.ithome.com/0/975/865.htm)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*