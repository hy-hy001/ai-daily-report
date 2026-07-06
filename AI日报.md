# AI 日报精选 TOP 10
**2026-07-06** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. 扎克伯格：建千兆瓦级AI集群，集中精英与资本
🔴 评分 **84** · X：Rohan Paul (@rohanpaul_ai) · 17 小时前

> "我们正在建设这个 Prometheus 集群，首个千兆瓦以上的单一集群……我们是在谈论数千亿美元的资本投入。"

Mark Zuckerberg 表示，他的职责就是集中精英人才、资本和基础设施。

🔗 [阅读原文](https://x.com/rohanpaul_ai/status/2073834219659534816)

---

### 2. pxpipe：通过图像化压缩输入token降低Claude Code成本
🔴 评分 **83** · Hacker News 热门（buzzing.cc 中文翻译） · 2 天前

> pxpipe是一个本地代理，将系统提示、工具文档和历史记录等密集文本渲染为PNG图像，利用图像token成本取决于像素尺寸的特性压缩输入token。在Fable 5模型上，约25k文本token压缩为约2.7k图像token，端到端账单降低59-70%。SWE-bench Lite 10个实例全部通过，成本从$54降至$27；SWE-bench Pro 19对测试中18对判定一致，单次请求成本降低约60%。该方法有损（精确ID等需保持文本），默认仅处理`claude-fable-5`请求，可通过`PXPIPE_MODELS`变量控制。

🔗 [阅读原文](https://github.com/teamchong/pxpipe)

---

### 3. 美团 LongCat-2.0 完全开源（MIT 许可），1.6T MoE 模型开放权重与推理代码
🔴 评分 **81** · X：美团 LongCat (@Meituan_LongCat) · 21 小时前

> 美团今日宣布 LongCat-2.0 完全开源（MIT 许可），公开模型权重与推理代码。该模型为 MoE 架构，总参数量 1.6T，每 token 激活约 48B，支持 1M token 上下文。技术亮点包括 LongCat Sparse Attention 高效处理长文本、Zero-Compute Experts 动态激活 33B-56B 零浪费计算、MOPD 按任务路由 Agent/Reasoning/Interaction 三组专家。Benchmark 成绩：Terminal-Bench 2.1 70.8；SWE-bench Pro 59.5（超越 GPT-5.5 的 58.6）；SWE-bench Multilingual 77.3；FORTE 73.2；RWSearch 78.8；BrowseComp 79.9。原生集成 Claude Code、OpenClaw、Hermes Agent 等工具，支持 GPU 与 NPU 部署，已在大规模国内集群验证。

🔗 [阅读原文](https://x.com/Meituan_LongCat/status/2073768940078317713)

---

### 4. claude-real-video ─ 让任何大语言模型（LLM）都能观看视频
🔴 评分 **81** · Hacker News 热门（buzzing.cc 中文翻译） · 3 天前

> claude-real-video 是一个开源工具，让大语言模型基于视频画面而非字幕进行理解。它通过场景变化检测提取关键帧、滑动窗口去重并转录音频，生成干净的本地文件夹供模型读取。支持 YouTube 链接或本地文件，依赖 ffmpeg 和 Whisper，通过 pip 安装。全部处理在本地完成，不上传云端。

🔗 [阅读原文](https://github.com/HUANGCHIHHUNGLeo/claude-real-video)

---

### 5. 阿里达摩院发布超导材料发现AI智能体Elements Claw
🔴 评分 **80** · IT之家（RSS） · 3 天前

> 7月3日，阿里达摩院联合中国人民大学、中国科学院大学发布首个超导材料发现AI智能体Elements Claw。该智能体采用"专通融合"架构，基于1.25亿分子/晶体结构预训练的1B参数原子基础模型Elements，判断超导性AUC达0.996，预测临界温度平均误差小于1K。AI仅用28个GPU小时筛选240万晶体结构，预测出6.8万个候选材料，其中4种（Hf21Re25、Zr4VRe7、HfZrRe4、Zr3ScRe8）已合成并验证超导性，临界温度最高6.5K。全部240万稳定晶体数据库已开放。

🔗 [阅读原文](https://www.ithome.com/0/972/089.htm)

---

### 6. 国家网信办就《互联网信息服务管理办法》再次征求意见，首设"智能信息服务"专章规范AI服务
🟠 评分 **79** · IT之家（RSS） · 3 天前

> 7月3日，国家互联网信息办公室就《互联网信息服务管理办法（修订草案征求意见稿）》再次公开征求意见。草案新增"智能信息服务"专章，要求AI服务提供者公示技术基本原理、训练数据来源，对生成合成内容进行标识，禁止强制用户使用智能服务或利用算法扰乱网络舆论。草案还强化用户账号管理，明确对超过6个月不登录账号可依约注销；要求平台建立网络暴力信息特征库，提供屏蔽、禁止转载等防护选项。意见反馈截止8月2日。

🔗 [阅读原文](https://www.ithome.com/0/972/341.htm)

---

### 7. browser-use 发布开源 AI 视频剪辑 Skill「video-use」
🟠 评分 **79** · X：邵猛 (@shao__meng) · 3 天前

> browser-use 团队推出面向 Codex、Claude Code 等 AI 编码智能体的开源 Skill「video-use」，让 LLM 通过 ElevenLabs Scribe 将音频转写为约 12KB 文本（含逐词时间戳、说话人分离、事件标记），仅在决策点调用 timeline_view.py 生成 PNG 帧图。技术流水线包括转写、打包、生成 JSON 格式 EDL、ffmpeg 渲染及最多 3 轮自评估。渲染关键细节：分段提取 + `-c copy` 拼接、30ms 音频淡入淡出、PTS 时移、字幕最后叠加、HDR 自动映射、竖屏缩放、两-pass loudnorm。动画支持 HyperFrames、Remotion、Manim 等引擎。项目附带 12 条硬规则确保生产正确性。

🔗 [阅读原文](https://x.com/shao__meng/status/2072644710523691110)

---

### 8. Microsoft 成立"Frontier Company"，斥资 25 亿美元派驻 6000 名 AI 工程师到企业客户现场
🟠 评分 **78** · The Decoder：AI News（RSS） · 3 天前

> Microsoft 新设业务部门"Frontier Company"，拨款 25 亿美元，将 6000 名行业与工程专家派驻企业客户现场，"共同设计、共同创新、部署并持续改进 AI 系统"。该部门由 Rodrigo Kede Lima 领导，旨在超越"前部署工程"模式，成为"最大、以结果为导向的工程组织"。Microsoft 将自己定位为 OpenAI 和 Anthropic 的"平台中立"替代方案，后两者也已设立专门部署公司。Microsoft 将借助埃森哲、凯捷、安永等系统集成商扩大覆盖范围。

🔗 [阅读原文](https://the-decoder.com/microsoft-launches-2-5-billion-frontier-company-to-embed-6000-ai-engineers-inside-enterprise-clients)

---

### 9. Wan Video 推出"音乐伴舞"新功能
🟠 评分 **77** · X：阿里云 / Alibaba Cloud (@alibaba_cloud) · 3 天前

> Wan Video 新功能：**音乐伴舞** 💃
上传一个角色，添加一首歌曲，让 Wan Video 生成与节奏同步的舞蹈视频。
可用舞种：
• 街舞
• 踢踏舞
• 拉丁舞
• K-Pop
• 中国古典舞
从节拍至动作，你的角色随音乐起舞。

前往 wan.video 体验音乐伴舞 👉 https://int.alibabacloud.com/m/1000412428/

🔗 [阅读原文](https://x.com/alibaba_cloud/status/2072967570441834771)

---

### 10. 关于Mythos和网络安全的讨论并非炒作
🟠 评分 **77** · X：Ethan Mollick (@emollick) · 3 天前

> 关于Mythos和网络安全的讨论并非炒作。
（正如任何使用Fable进行自主工作的人可能已经认识到的那样。）

🔗 [阅读原文](https://x.com/emollick/status/2072778376494895139)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*