# AI 日报精选 TOP 10
**2026-07-07** | 数据来源：[AIHOT](https://aihot.virxact.com)

---

### 1. 语言模型中的全局工作空间
🔴 评分 **90** · Anthropic：Research（发表成果 · 网页） · 1 天前

> Anthropic在Claude中发现一组名为J-space的内部神经模式，类似神经科学的全局工作空间。每个模式关联特定词汇，但模型不必说出该词即可激活。Claude能报告J-space中的表征，并可应要求调节（如"在脑中思考"时点亮对应模式）。J-space还用于多步推理的中间步骤，且灵活支持多种任务（如从"法国"联想首都、货币等）。去除J-space后Claude仍能正常对话，但丧失高阶认知功能。该发现可用于监测模型私下察觉测试、生成虚假数据或执行隐藏目标。

🔗 [阅读原文](https://www.anthropic.com/research/global-workspace)

---

### 2. 扎克伯格：建千兆瓦级AI集群，集中精英与资本
🔴 评分 **84** · X：Rohan Paul (@rohanpaul_ai) · 1 天前

> "我们正在建设这个 Prometheus 集群，首个千兆瓦以上的单一集群……我们是在谈论数千亿美元的资本投入。"

Mark Zuckerberg 表示，他的职责就是集中精英人才、资本和基础设施。

🔗 [阅读原文](https://x.com/rohanpaul_ai/status/2073834219659534816)

---

### 3. pxpipe：通过图像化压缩输入token降低Claude Code成本
🔴 评分 **83** · Hacker News 热门（buzzing.cc 中文翻译） · 3 天前

> pxpipe是一个本地代理，将系统提示、工具文档和历史记录等密集文本渲染为PNG图像，利用图像token成本取决于像素尺寸的特性压缩输入token。在Fable 5模型上，约25k文本token压缩为约2.7k图像token，端到端账单降低59-70%。SWE-bench Lite 10个实例全部通过，成本从$54降至$27；SWE-bench Pro 19对测试中18对判定一致，单次请求成本降低约60%。该方法有损（精确ID等需保持文本），默认仅处理`claude-fable-5`请求，可通过`PXPIPE_MODELS`变量控制。

🔗 [阅读原文](https://github.com/teamchong/pxpipe)

---

### 4. 美团 LongCat-2.0 完全开源（MIT 许可），1.6T MoE 模型开放权重与推理代码
🔴 评分 **81** · X：美团 LongCat (@Meituan_LongCat) · 1 天前

> 美团今日宣布 LongCat-2.0 完全开源（MIT 许可），公开模型权重与推理代码。该模型为 MoE 架构，总参数量 1.6T，每 token 激活约 48B，支持 1M token 上下文。技术亮点包括 LongCat Sparse Attention 高效处理长文本、Zero-Compute Experts 动态激活 33B-56B 零浪费计算、MOPD 按任务路由 Agent/Reasoning/Interaction 三组专家。Benchmark 成绩：Terminal-Bench 2.1 70.8；SWE-bench Pro 59.5（超越 GPT-5.5 的 58.6）；SWE-bench Multilingual 77.3；FORTE 73.2；RWSearch 78.8；BrowseComp 79.9。原生集成 Claude Code、OpenClaw、Hermes Agent 等工具，支持 GPU 与 NPU 部署，已在大规模国内集群验证。

🔗 [阅读原文](https://x.com/Meituan_LongCat/status/2073768940078317713)

---

### 5. claude-real-video ─ 让任何大语言模型（LLM）都能观看视频
🔴 评分 **81** · Hacker News 热门（buzzing.cc 中文翻译） · 3 天前

> claude-real-video 是一个开源工具，让大语言模型基于视频画面而非字幕进行理解。它通过场景变化检测提取关键帧、滑动窗口去重并转录音频，生成干净的本地文件夹供模型读取。支持 YouTube 链接或本地文件，依赖 ffmpeg 和 Whisper，通过 pip 安装。全部处理在本地完成，不上传云端。

🔗 [阅读原文](https://github.com/HUANGCHIHHUNGLeo/claude-real-video)

---

### 6. 阿里达摩院发布超导材料发现AI智能体Elements Claw
🔴 评分 **80** · IT之家（RSS） · 3 天前

> 7月3日，阿里达摩院联合中国人民大学、中国科学院大学发布首个超导材料发现AI智能体Elements Claw。该智能体采用"专通融合"架构，基于1.25亿分子/晶体结构预训练的1B参数原子基础模型Elements，判断超导性AUC达0.996，预测临界温度平均误差小于1K。AI仅用28个GPU小时筛选240万晶体结构，预测出6.8万个候选材料，其中4种（Hf21Re25、Zr4VRe7、HfZrRe4、Zr3ScRe8）已合成并验证超导性，临界温度最高6.5K。全部240万稳定晶体数据库已开放。

🔗 [阅读原文](https://www.ithome.com/0/972/089.htm)

---

### 7. 国家网信办就《互联网信息服务管理办法》再次征求意见，首设"智能信息服务"专章规范AI服务
🟠 评分 **79** · IT之家（RSS） · 3 天前

> 7月3日，国家互联网信息办公室就《互联网信息服务管理办法（修订草案征求意见稿）》再次公开征求意见。草案新增"智能信息服务"专章，要求AI服务提供者公示技术基本原理、训练数据来源，对生成合成内容进行标识，禁止强制用户使用智能服务或利用算法扰乱网络舆论。草案还强化用户账号管理，明确对超过6个月不登录账号可依约注销；要求平台建立网络暴力信息特征库，提供屏蔽、禁止转载等防护选项。意见反馈截止8月2日。

🔗 [阅读原文](https://www.ithome.com/0/972/341.htm)

---

### 8. 2026年科技公司AI裁员名单：Microsoft、Oracle、GitLab等十家公司裁减数千岗位
🟠 评分 **78** · TechCrunch：AI（RSS） · 4 小时前

> 2026年以来，多家科技公司以AI为由大规模裁员。Microsoft裁减约4800岗位（2.1%），Oracle裁减21000人（13%），GitLab裁减350人（14%）以投资AI基础设施，Google Cloud持续裁减员工（外界估计1500-3000+工程师），Intuit裁减3000人（17%），Meta裁减8000人（10%）并转岗7000人至AI，Cisco裁减近4000人（5%），Cloudflare裁减1100人（20%），GM裁减500-600 IT岗位，Coinbase裁减700人（14%）。据Layoffs.fyi统计，2026年累计已裁约12万个技术岗位。

🔗 [阅读原文](https://techcrunch.com/2026/07/06/the-running-list-major-tech-layoffs-in-2026-where-employers-cited-ai)

---

### 9. Microsoft 成立"Frontier Company"，斥资 25 亿美元派驻 6000 名 AI 工程师到企业客户现场
🟠 评分 **78** · The Decoder：AI News（RSS） · 4 天前

> Microsoft 新设业务部门"Frontier Company"，拨款 25 亿美元，将 6000 名行业与工程专家派驻企业客户现场，"共同设计、共同创新、部署并持续改进 AI 系统"。该部门由 Rodrigo Kede Lima 领导，旨在超越"前部署工程"模式，成为"最大、以结果为导向的工程组织"。Microsoft 将自己定位为 OpenAI 和 Anthropic 的"平台中立"替代方案，后两者也已设立专门部署公司。Microsoft 将借助埃森哲、凯捷、安永等系统集成商扩大覆盖范围。

🔗 [阅读原文](https://the-decoder.com/microsoft-launches-2-5-billion-frontier-company-to-embed-6000-ai-engineers-inside-enterprise-clients)

---

### 10. AI颠覆初级程序员就业市场：斯坦福数据揭示年轻开发者就业锐减19%
🟠 评分 **77** · Hacker News 热门（buzzing.cc 中文翻译） · 11 小时前

> 斯坦福数字经济实验室基于ADP薪资数据发现，美国22-25岁软件开发人员就业较2022年峰值下降19%，而41-49岁增长14%。入门级岗位招聘减少28%，计算机科学毕业生失业率达6.1%，高于文科专业。核心推手是2024-2025年兴起的智能体编程（Agentic programming）。总程序员就业增长4.4%，但全部来自年长群体。GitHub一年新增3600万账号，80%新用户一周内使用Copilot。编程工作未消失，但"初级程序员"头衔正在消亡。

🔗 [阅读原文](https://seldo.com/posts/ai-has-torched-the-market-for-junior-programmers)

---


*每日自动生成，覆盖前一天内容。由 aihot.virxact.com 提供数据支持。*