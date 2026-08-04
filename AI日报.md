# AI 日报精选 TOP 10
**2026-08-05** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. Qwen3.8-Max 发布：开源最强编码与协作模型，2.4T 参数
🔴 评分 **89** · Qwen：Blog Retrieval（API） · 1 天前

> Qwen 正式发布 Qwen3.8-Max，这是 Qwen 家族迄今最强的模型，拥有 2.4T 参数（95B 激活），并首次开源 Qwen-Max 级权重，开放权重将于下周发布。

🔗 [阅读原文](https://qwen.ai/blog?id=qwen3.8)

---

### 2. Swiftlet：在 Mac 上运行 80B 版 Qwen（内存 4.3 GB），在 iPhone 上运行 35B 版
🔴 评分 **81** · Hacker News 热门（buzzing.cc 中文翻译） · 16 小时前

> Swiftlet 是一个 Swift + Metal 运行时，可在普通 Apple 设备上运行 Qwen3-Next 和 Qwen3.5/3.6 MoE 混合模型，仅将小型稠密核心驻留内存，按需从存储流式加载路由专家权重。

🔗 [阅读原文](https://github.com/leonickson1/Swiftlet)

---

### 3. Reflex 开源 XY：基于 Rust 的超快 Python 绘图库，可保持 1 亿点图表交互流畅
🟠 评分 **79** · MarkTechPost（RSS） · 14 小时前

> Reflex AI 发布 Apache-2.0 许可的 Python 交互式 2D 绘图库 XY，通过 Rust 原生核心、二进制缓冲传输和 WebGL2 渲染，在 1 万至 1 亿点范围内保持约 0.08 秒的渲染时间。

🔗 [阅读原文](https://www.marktechpost.com/2026/08/04/reflex-open-sources-xy-a-rust-backed-super-fast-python-charting-library-that-keeps-100-million-point-charts-interactive)

---

### 4. Anthropic 与成立仅数月的云初创公司 Volta 签署 100 亿美元算力协议
🟠 评分 **78** · X：Rohan Paul (@rohanpaul_ai) · 8 小时前

> Anthropic 与成立仅数月的云初创公司 Volta 签署 100 亿美元算力协议，约合每年 17 亿美元。Volta 估值 24 亿美元，硬件几乎全为租用：算力来自比特币矿商 Bitdeer 挪威 121MW 站点，芯片由 Nvidia 供应、Dell 组装。Anthropic 买的是交付速度，代价是承担超大规模云厂商合同从未有过的交易对手风险。

🔗 [阅读原文](https://x.com/rohanpaul_ai/status/2084655258102546579)

---

### 5. 面壁智能开源 ForgeStencil：一周自动优化 100+ 工业与科学软件，全程零人工介入
🟠 评分 **78** · 公众号：面壁智能（MiniCPM） · 18 小时前

> 面壁智能联合 OpenBMB 开源全球首个支持 Stencil 自动研究、自动部署的 AI 优化系统 ForgeStencil，由 Kernel Agent 与 App Agent 闭环协作，实现从算子优化到应用集成的全自动流程。

🔗 [阅读原文](https://mp.weixin.qq.com/s?__biz=Mzg3Mzg2MTg2NQ%3D%3D&mid=2247498861&idx=1&sn=d2d16692dd7eb27f9d466803f25c2b78)

---

### 6. 在单颗 AMD MI300X 上运行 DeepSeek V4 Flash
🟠 评分 **76** · Hacker News 热门（buzzing.cc 中文翻译） · 10 小时前

> 一个开源仓库提供了在单颗 AMD MI300X 上生产运行 DeepSeek-V4-Flash-0731 的完整配置与补丁，无需额外量化或权重卸载。该 304B 参数模型在 192 GB HBM 上实现单流 168.6 tok/s 解码、8 并发流 542 tok/s 聚合吞吐，并验证了 256K 上下文。

🔗 [阅读原文](https://github.com/ryanzhou/deepseek-v4-flash-mi300x)

---

### 7. AirLLM 实现单块 4GB GPU 运行 70B 模型推理
🟠 评分 **76** · Hacker News 热门（buzzing.cc 中文翻译） · 1 天前

> AirLLM 项目支持在单块 4GB 显存 GPU 上运行 70B 参数大模型推理，无需多卡或大规模显存配置。该项目已开源，相关讨论在 Hacker News 上获得 103 点热度，引发社区关注。

🔗 [阅读原文](https://github.com/lyogavin/airllm)

---

### 8. MiniMax H3 正式开源：通用全模态生成系统支持 2K 视频与原生立体声
🟠 评分 **75** · 公众号：MiniMax（稀宇科技） · 1 天前

> MiniMax 正式开源新一代通用视频模型 H3，可统一理解文本、图像、视频和音频，生成最高 2K 分辨率、最长 15 秒、带 32 kHz 原生立体声音频的视频。

🔗 [阅读原文](https://mp.weixin.qq.com/s?__biz=MzE5MTA3NzcxMQ%3D%3D&mid=2247488931&idx=1&sn=0506e1d52edd5166becf35f5ebd83a07)

---

### 9. Codex 用 Sol 指挥 Luna Max 省额度翻倍产出
🟠 评分 **75** · X：阿易 AI Notes (@AYi_AInotes) · 2 天前

> Codex 高阶玩法：让 Sol 在 `~/.codex/agents/` 下创建 `luna-worker.toml` 子代理，模型设 `gpt-5.6-luna`、reasoning effort 设 max，Sol 负责拆任务与审代码，具体实现自动委托给 Luna Max。

🔗 [阅读原文](https://x.com/AYi_AInotes/status/2083867265179537565)

---

### 10. MiniMax-H3 通过 MLX 移植可在 Apple Silicon 上运行
🟠 评分 **74** · Simon Willison 博客 · 3 小时前

> MiniMax 发布 MiniMax-H3，一个可接受文本、图像、音频和视频并生成最长 15 秒带音频视频片段的通用全模态生成系统。Python 包 PipeNetwork/minimax-h3-mlx 将其移植到 MLX，支持 Apple Silicon 运行。作者在 M5 Max MacBook Pro 上实测，下载约 115 GB 模型文件，视频生成耗时不到 45 分钟。

🔗 [阅读原文](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*