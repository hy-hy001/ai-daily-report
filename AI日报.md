# AI 日报精选 TOP 10
**2026-07-10** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. GitLost：Noma Labs 发现 GitHub AI 代理提示词注入漏洞
🔴 评分 **81** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> Noma Labs 在 GitHub Agentic Workflows 中发现严重提示词注入漏洞 GitLost。未认证攻击者仅需在属于同一组织的公共仓库中创建一个嵌有恶意指令的 Issue，即可诱使基于 Claude 或 GitHub Copilot 的 AI 代理读取并公开该组织内私有仓库的内容。攻击无需编码技能或凭证，根源在于代理将用户可控内容视为可信指令，且 GitHub 的防护措施因 "Additionally" 关键词被绕过。Noma Labs 已公开 PoC 并建议限制跨仓库权限、隔离用户输入。

🔗 [阅读原文](https://noma.security/blog/gitlost-how-we-tricked-githubs-ai-agent-into-leaking-private-repos)

---

### 2. OpenAI 推出 ChatGPT Work：可跨应用自主工作的 AI 智能体
🔴 评分 **80** · OpenAI：官网动态（RSS · 排除企业/客户案例） · 13 小时前

> OpenAI 发布 ChatGPT Work，一个能跨应用和文件收集信息、将复杂项目分解为小步骤独立完成并持续工作数小时的 AI 智能体。它内置 Codex 技术，目前每周超 500 万用户使用 Codex，其中超 100 万用于非软件开发场景。ChatGPT Work 由今天同步推出的最新前沿模型 GPT-5.6 驱动，具备多步骤推理和按模板生成材料的能力。该功能今天起面向 Pro、Enterprise 和 Edu 计划推出，未来几天扩展至 Plus 和 Business 计划。桌面版 ChatGPT 在所有计划（含免费版）中提供 Chat、Work 和 Codex 模式，且 Codex 应用已合并至新的桌面应用。

🔗 [阅读原文](https://openai.com/index/chatgpt-for-your-most-ambitious-work)

---

### 3. Claude开发者分享两种多智能体模式：Advisor和Orchestrator
🔴 评分 **80** · X：邵猛 (@shao__meng) · 1 天前

> Claude开发者官方分享团队高频使用的两种多智能体模式。Advisor模式：Sonnet 5作为执行者，通过tool call调用Fable 5获取指导。SWE-bench Pro（482题）上，Sonnet 5单独75.5%/$0.75，加顾问达84%/$1.40，Fable 5单独91.5%/$2.25；组合方案约92%性能、63%成本。Orchestrator模式：Fable 5作为编排者规划并向多个Sonnet 5 worker扇出任务。BrowseComp上，全Sonnet 5 77.8%/$16.01，编排方案86.8%/$18.53，全Fable 5 90.8%/$40.56；编排方案约96%性能、46%成本。

🔗 [阅读原文](https://x.com/shao__meng/status/2074661249804366310)

---

### 4. 推出 Grok 4.5
🔴 评分 **80** · Cursor Blog · 1 天前

> Cursor 与 SpaceXAI 联合训练了混合专家模型 Grok 4.5，在数万亿 tokens 的 Cursor 用户交互数据上训练，并通过强化学习解决软件工程、数据科学、金融、法律等领域的困难问题。基础版定价 $2/M 输入 tokens、$6/M 输出 tokens，快速版 $4/M 输入 tokens、$18/M 输出 tokens。即日起在 Cursor 桌面、网页、iOS、CLI 及 SDK 中可用，个人和团队计划首周使用量翻倍。Grok 4.5 与 Composer 2.5 为不同权重类别，两者将继续支持。

🔗 [阅读原文](https://cursor.com/blog/grok-4-5)

---

### 5. 工信部发布Claude Code后门安全风险提示
🟠 评分 **79** · X：小互 (@xiaohu) · 1 天前

> 中国工信部发布风险提示，指出 Claude Code 2.1.91 至 2.1.196 版本内置监控机制，未经用户同意即向远程服务器回传用户地域、身份标识等敏感信息。建议相关单位立即全面排查，对受影响版本卸载或升级至已清除后门代码的最新安全版本，并加强开发工具外联权限管控与流量监测，防止敏感数据违规外传。

🔗 [阅读原文](https://x.com/xiaohu/status/2074736623284256881)

---

### 6. 黑客可利用9款最流行的AI工具组装大规模僵尸网络
🟠 评分 **78** · Ars Technica：AI（RSS） · 1 天前

> 提示注入已成为AI安全的首要威胁--大语言模型无法区分合法指令与恶意指令。此前推送式和拉取式攻击规模均有限。研究人员提出一种名为HalluSquatting的新型拉取式提示注入攻击，首次能组装大规模僵尸网络、执行分布式拒绝服务攻击（DDoS）并大规模感染设备。该攻击可作用于AI编码工具，标志着提示注入攻击从单点突破转向规模化利用。

🔗 [阅读原文](https://arstechnica.com/security/2026/07/hackers-can-use-9-of-the-most-popular-ai-tools-to-assemble-massive-botnets)

---

### 7. OpenAI 发布 GPT-Live 新一代全双工语音模型
🟠 评分 **77** · OpenAI：官网动态（RSS · 排除企业/客户案例） · 1 天前

> OpenAI 今日推出 GPT-Live，基于全双工架构实现同时听与说，支持自然打断与实时回馈。该模型每秒多次判断是否说话、倾听、打断或调用工具，并将搜索、推理等复杂任务委托给后台 GPT-5.5，保持对话流畅。即日起向全球 ChatGPT 用户提供 GPT-Live-1 和 GPT-Live-1 mini 两个版本。人类评估显示，在 5-10 分钟对话中，GPT-Live-1 系列在自然度、轮流、打断等方面显著优于 Advanced Voice Mode；在 GPQA、BrowseComp 和 τ3-Voice Telecom 基准测试中也表现更强。未来将开放 API。

🔗 [阅读原文](https://openai.com/index/introducing-gpt-live)

---

### 8. 在校研究生Kunkun开源管理相互调用Skill的方法
🟠 评分 **76** · X：Berry Xia (@berryxia) · 1 天前

> 在校研究生Kunkun开源了一套管理大量互相调用Skill的方法。核心方案包括：1）搭建HTML后台，按运行模式（手动/自动）、链路位置、专业领域三类标签筛选Skill；2）将连环调用的Skill绘制成Mermaid流程图，根据debug、新功能、合PR、改设计等阶段定位对应技能组；3）仿照Matt的ask Matt技能开发"ask me"技能，将调用决策浓缩成上下文喂给模型。该方法避免将所有调用交给模型自行判断，保持工程复杂场景下的人机对齐与可控性。项目已开源至GitHub。

🔗 [阅读原文](https://x.com/berryxia/status/2074827915779580055)

---

### 9. 微软发布Flint：面向AI智能体的可视化语言
🟠 评分 **75** · Hacker News 热门（buzzing.cc 中文翻译） · 1 小时前

> 微软研究院推出Flint，一种可视化中间语言，让AI智能体通过简洁的人类可编辑spec自动生成美观图表。用户只需提供数据、语义类型和图表类型，Flint编译器即可推导坐标轴、配色、布局等底层参数。支持46种图表类型，可渲染到Vega-Lite、ECharts和Chart.js三个后端。项目通过npm安装（TypeScript/JavaScript），并提供MCP服务器用于智能体工作流集成。采用弹性布局模型自动优化图表尺寸与间距，已开源。

🔗 [阅读原文](https://microsoft.github.io/flint-chart)

---

### 10. 加拿大不列颠哥伦比亚省拟起诉OpenAI：未上报ChatGPT暴力对话致校园枪击惨案
🟠 评分 **75** · IT之家（RSS） · 1 天前

> 加拿大不列颠哥伦比亚省7月7日宣布将起诉OpenAI，指控其未向执法部门上报一名ChatGPT用户2025年6月封禁前的暴力相关对话内容。该用户随后于今年2月在塔布勒岭制造校园枪击案，杀害8人。OpenAI CEO萨姆·奥尔特曼今年4月为此公开致歉，承认本应上报但未执行。受害家属已在加州法院提起诉讼，省政府正协调独立诉讼，要求赔偿用于社区重建。

🔗 [阅读原文](https://www.ithome.com/0/974/169.htm)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*