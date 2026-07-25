# AI 日报精选 TOP 10
**2026-07-26** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. Anthropic 发布 Claude Opus 5
🔴 评分 **92** · Anthropic：Newsroom（网页） · 2 天前

> Anthropic 发布 Claude Opus 5，其智能水平接近 Claude Fable 5，但价格减半。该模型在 Frontier-Bench v0.1 上性能超过 Opus 4.8 两倍以上，在 ARC-AGI 3 上得分是次优模型的三倍。Opus 5 即日起成为 Claude Max 的默认模型和 Claude Pro 的最强模型。

🔗 [阅读原文](https://www.anthropic.com/news/claude-opus-5)

---

### 2. Anthropic 因盗版书籍支付 15 亿美元和解金，创下集体诉讼版权赔偿纪录
🔴 评分 **86** · The Decoder：AI News（RSS） · 3 天前

> Anthropic 向图书作者支付 15 亿美元版权和解金，联邦法院已批准。约 482460 部作品中 91.3% 被索赔，每部约获 3000 美元。法官此前裁定，在合法获取的书籍上训练 AI 属于"变革性"合理使用，但大规模抓取网络内容是否合法仍悬而未决。

🔗 [阅读原文](https://the-decoder.com/anthropics-1-5b-piracy-settlement-with-book-authors-is-a-record-loss-that-hands-ai-labs-their-biggest-legal-win)

---

### 3. Claude-thermos：保持 Claude 会话缓存热度，避免重新编码费用
🟠 评分 **79** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> Claude-thermos 通过本地反向代理监控 Claude Code 会话，在主智能体因等待子智能体而空闲超过 5 分钟时，自动发送预热请求刷新提示缓存。实测约 185 次本地会话中，缓存过期导致的重新编码占账单约 22%。工具以 uvx 运行，支持自定义空闲阈值和预热间隔。

🔗 [阅读原文](https://github.com/izeigerman/claude-thermos)

---

### 4. ChatGPT 桌面版上线语音控制多智能体
🟠 评分 **79** · X：OpenAI (@OpenAI) · 2 天前

> ChatGPT 语音功能现已登陆桌面应用。

只需使用语音，即可控制你的电脑，并指挥在 ChatGPT Work 或 Codex 中运行的多个智能体。

该功能由 GPT-Live 驱动，因此它能够同时在该应用中说话、聆听并协调工作。

今日起，面向 macOS 和 Windows 平台的 Plus、Pro、Business、Edu 及 Enterprise 计划用户全球推送。

🔗 [阅读原文](https://x.com/OpenAI/status/2080378182469857576)

---

### 5. 通义千问发布Qwen-Audio-3.0-TTS，登顶TTS排行榜
🟠 评分 **79** · X：通义千问 / Qwen (@Alibaba_Qwen) · 2 天前

> 阿里通义千问推出最新文本转语音模型Qwen-Audio-3.0-TTS，提供Flash（实时交互）和Plus（高质量生成）两个版本。新功能包括细粒度内联标签控制（如【whisper】、【angry】）、自然语言风格控制、支持16种语言，以及一次生成长达3分钟的长文本。该模型目前在Artificial Analysis TTS排行榜上排名第一。

🔗 [阅读原文](https://x.com/Alibaba_Qwen/status/2080270065547809133)

---

### 6. AREX：面向深度研究的递归自改进智能体
🟠 评分 **78** · HuggingFace Daily Papers（社区热门论文） · 2 天前

> AREX 是一系列递归自改进（RSI）深度研究智能体，通过内层研究循环收集证据、外层自改进循环逐约束审计答案并启动针对性研究。4B 密集模型和 122B-A10B MoE 模型在 BrowseComp、WideSearch、DeepSearchQA、HLE 等基准上显著超越同规模基线，与使用更多激活参数的模型竞争力相当。

🔗 [阅读原文](https://arxiv.org/abs/2607.21461)

---

### 7. 英伟达、微软和Meta联合警告：应避免对开放权重模型过度监管
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> 英伟达、微软和Meta联合签署公开信，警告对开放权重AI模型的过度监管将削弱美国在AI领域的竞争力。信中指出，开放权重模型能促进创新、降低准入门槛，并支持学术研究。OpenAI和Anthropic未签署该信函。

🔗 [阅读原文](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html)

---

### 8. 佛州男子因相信 ChatGPT 拒绝就医而险些丧命，起诉 OpenAI 及 CEO 奥尔特曼
🟠 评分 **77** · IT之家（RSS） · 1 天前

> 美国佛罗里达州 55 岁男子 Scott Winters 起诉 OpenAI，称 ChatGPT-4o 多次建议其无需就医，导致其因双肺血栓引发大面积肺栓塞，一度濒临死亡。诉状指控 OpenAI 存在疏忽和"无证行医"行为，要求经济赔偿并暂停 ChatGPT Health 服务。OpenAI 回应称 ChatGPT 不是医生，不应替代专业医疗护理。

🔗 [阅读原文](https://www.ithome.com/0/980/890.htm)

---

### 9. 小红书HELMSMAN：全闪存服务器实现高性能向量检索，硬件成本节省超90%
🟠 评分 **77** · 公众号：小红书技术（dots.llm） · 2 天前

> 小红书引擎架构团队在OSDI 2026提出HELMSMAN，一个面向全闪存服务器的高性能向量近似最近邻搜索系统。该系统通过聚类式索引、定制化存储栈和分层学习式搜索剪枝，用约40台全闪存服务器承载了过去约35，000 CPU Core和约350 TB DRAM的负载，硬件成本节省超过90%。

🔗 [阅读原文](https://mp.weixin.qq.com/s/WCYE6itbTBPU0Q_3BfQxkA)

---

### 10. SANA-Video 2.0：混合线性注意力与注意力残差实现高效视频生成
🟠 评分 **77** · HuggingFace Daily Papers（社区热门论文） · 2 天前

> SANA-Video 2.0 是一个混合视频扩散 Transformer，提供 5B 和 14B 两种规模，可在单 GPU 上生成最高 720p 视频。其 Hybrid Linear-Softmax Attention 以 3：1 比例混合线性与 softmax 注意力，配合 Block Attention Residuals 将深层有效秩提升约 12%。

🔗 [阅读原文](https://arxiv.org/abs/2607.21553)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*