# AI 日报精选 TOP 10
**2026-07-14** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. xAI 官方 Grok CLI 被曝静默上传整个代码库及用户密钥
🔴 评分 **86** · 公众号：数字生命卡兹克 · 22 小时前

> 安全研究者发现，xAI 官方 Grok CLI（npm 包 `@xai-official/grok` 0.2.93 版）会在每轮任务前后，将当前工作目录打包为 `before_codebase.tar.gz` 和 `after_codebase.tar.gz`，通过独立旁路通道静默上传至 xAI 的 Google Cloud 仓库。验证显示，即使模型仅回复一个单词，上传依然发生。上传包还包含仓库外的 `~/.claude.json`、Claude Code 设置、全局 AGENTS 规则、30 多个 Skill 文件及一个 API 密钥。7 月 13 日凌晨，xAI 通过服务端远程开关新增 `disable_codebase_upload` 字段，将默认上传行为关闭，但此前该功能默认开启。

🔗 [阅读原文](https://mp.weixin.qq.com/s/6c6vGMJAVMbh6UhNVw4dcg)

---

### 2. 苹果起诉OpenAI窃取商业机密开发AI硬件
🔴 评分 **84** · X：宝玉 (@dotey) · 3 天前

> 苹果公司今日在加州北区联邦地方法院对OpenAI提起诉讼，指控其系统性窃取苹果商业机密，用于开发AI硬件设备。被告包括OpenAI、其硬件负责人Tang Tan（前苹果iPhone和Apple Watch产品设计副总裁，在苹果任职24年）、前苹果高级系统电气工程师Chang Liu，以及Jony Ive联合创立的io Products。Jony Ive本人未被列为被告。

🔗 [阅读原文](https://x.com/dotey/status/2075712647723397452)

---

### 3. OpenAI 论文：GPT-5.6 Sol Ultra 证明图论"循环双覆盖猜想"
🔴 评分 **84** · Hacker News 热门（buzzing.cc 中文翻译） · 3 天前

> OpenAI 发布论文，称 GPT-5.6 Sol Ultra 证明了图论中悬而未决的"循环双覆盖猜想"。该猜想断言每个无桥无向图都存在一组环，每条边恰好被覆盖两次。论文利用 GPT-5.6 Sol Ultra 完成证明，并借助 Codex 撰写。证明过程首先将问题简化为三次图，利用 8-流定理和 Tutte 的结果将边标记为 F32 的非零元，再转化为每个顶点处每个元素出现零次或两次的二元集标记，最终归结为线性代数论证。

🔗 [阅读原文](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf)

---

### 4. 宇树G1人形机器人完成首例活体微创手术
🟠 评分 **79** · X：X.PIN (@thexpin) · 3 天前

> 一篇新的《自然》论文展示了宇树G1人形机器人执行研究人员所称的首例由人形机器人完成的活体标准微创手术。加州大学圣地亚哥团队使用G1，以常规手术器械完成了对两只活猪的腹腔镜胆囊切除术；第二次手术耗时32分钟。该机器人仍需反复校正，且尚无法满足手术无菌标准，但其成本可能仅为达芬奇系统的约5%。

🔗 [阅读原文](https://x.com/thexpin/status/2075640168896516139)

---

### 5. OpenAI 面向普通用户发布提示词指南：从结果出发，少写步骤
🟠 评分 **78** · The Decoder：AI News（RSS） · 5 小时前

> OpenAI 整合了一份面向普通用户的提示词指南，涵盖目标、上下文、输出格式和边界四个可选模块。指南建议以结果而非步骤开头，用一两条硬性规则替代逐步骤脚本。Chat 处理快速任务，基于 Codex 技术和 GPT-5.6 模型的 ChatGPT Work 负责多源、多步骤的复杂项目。Codex 新增 Steer（重定向当前运行）、Queue（排队下一条消息）和沙盒模式，支持 `/plan`、`/goal` 和 `/review` 等斜杠命令。用户无需一次性写对提示词，后续追问是预期调整方式。

🔗 [阅读原文](https://the-decoder.com/openais-new-prompting-guide-tells-users-to-stop-overthinking-and-start-with-the-result)

---

### 6. GenCeption：视频生成模型作为通用视觉学习器
🟠 评分 **78** · HuggingFace Daily Papers（社区热门论文） · 3 天前

> 论文提出 GenCeption，利用预训练文本到视频扩散模型作为前馈感知骨干，通过文本指令驱动完成深度估计、表面法线、相机位姿、指代分割和 3D 关键点预测等多种视觉任务。GenCeption 在多个基准上达到 SOTA，匹配或超越 DepthAnything3、SAM3、D4RT、VGGT-Omega 等专用模型。视频生成预训练骨干在同等设置下优于 V-JEPA 和 Video MAE 等替代范式。GenCeption 展现出数据与模型缩放特性，仅用 7 到 500 倍更少的训练数据即可达到 D4RT 和 VGGT-Omega 的同等性能。模型仅用合成人类视频训练，即可泛化到真实场景及动物、机器人等分布外物体类别。

🔗 [阅读原文](https://arxiv.org/abs/2607.09024)

---

### 7. 前沿模型实际成本：tokenizer 差异导致隐性涨价
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 1 小时前

> 同一份 TypeScript 文件在 GPT-5.x 上为 681 个 token，在 Claude 最新 tokenizer 下为 1，178 个，相差 1.73 倍。Anthropic 新 tokenizer 比旧版多产生约 30% 的 token，标价不变，构成隐性涨价。Claude Opus 4.6 与 Opus 4.8 标价同为 $5.00 / $25.00，但新 tokenizer 使同一代码的 token 数增加约 32%。Claude Sonnet 5 的 $2.00 / $10.00 为促销价，2026 年 8 月 31 日后恢复 $3.00 / $15.00，届时相同代码成本将比 Sonnet 4.6 高出约 32%。跨厂商对比中，Claude 新 tokenizer 在代码上比 GPT 多产生 1.50x 至 1.73x 的 token，TypeScript 差距最大。

🔗 [阅读原文](https://playcode.io/blog/real-price-of-frontier-models)

---

### 8. Meta 宣布扩建路易斯安那州数据中心至 5GW，总投资超 500 亿美元
🟠 评分 **77** · IT之家（RSS） · 12 小时前

> Meta 将其路易斯安那州数据中心算力扩至 5GW，总投资超 500 亿美元，为全球最大 AI 基础设施投资之一。Meta 承诺承担全部能源及水资源费用，并另投超 10 亿美元改善当地道路及供水系统。此外，Meta 与安特吉公司达成协议，为新建天然气发电厂、储能电池及核电增容项目提供资金支持。

🔗 [阅读原文](https://www.ithome.com/0/976/149.htm)

---

### 9. 黄仁勋：英伟达季度收入逼近千亿美元，Rubin Ultra 架构未延期
🟠 评分 **77** · IT之家（RSS） · 22 小时前

> 英伟达CEO黄仁勋在摩根士丹利路演中表示，公司季度营收即将逼近1000亿美元，且增长速度仍在加快。他否认下一代旗舰架构Rubin Ultra延期传闻，称其仍按计划于明年出货，当前机架设计调整仅为系统架构优化。一个此前主要依赖ASIC的前沿AI模型项目，如今英伟达GPU算力占比已接近50%，市场普遍指向Anthropic。英伟达预计本财年CPU业务收入约200亿美元，下一代Vera CPU将进军通用服务器市场。摩根士丹利维持英伟达"增持"评级，目标价288美元。

🔗 [阅读原文](https://www.ithome.com/0/975/865.htm)

---

### 10. Mesh LLM：在 iroh 上进行分布式人工智能计算
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> Mesh LLM 是一个开源项目，能将用户多台机器上的 GPU 和内存池化，对外暴露兼容 OpenAI 的 API。它通过 iroh 网络库实现点对点连接，无需中央服务器。请求可在本地 GPU 运行、路由到已加载模型的节点，或将大模型按层分区（内部称"Skippy"）流水线式拆分到多台机器。系统内置 40 多个模型，从 5 亿参数到 235B MoE 巨模型均可支持。软件体积约 18 MB，启动后以 `localhost：9337/v1` 提供服务。

🔗 [阅读原文](https://www.iroh.computer/blog/mesh-llm)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*