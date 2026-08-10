# HANDOVER — 高管对话四层框架 HTML 打磨（Codex）

> 交给 Codex 继续打磨的交接文档。
> 目标：把《高管对话 · 四层框架》做成一个能现场展示、且能继续演进的 HTML。
> 仓库：github.com/Jianan-Huang0609/Jianan-Career-Pathway
> 交接时间：2026-08-10

---

## 1. 背景与目标

Jianan 下周要跟公司高管 1v1 聊自己，希望用四层框架组织叙事：
① CER 项目（业务价值证明）→ ② AIDU Strategy（组织战略理解）→ ③ 个人职业发展（成长叙事）→ ④ 潜在答疑（1v1 提问清单）。

已有：本仓库 exec-talk/01-四层材料包.md（素材总集）、02-高管对话-展示.html（V1 展示版）。
本任务：把 02 HTML 打磨到可现场演示的质量，并把素材真正嵌进去。

## 2. 四层框架要点（每层素材源）

### Layer 1 · CER 项目
- 历程：FY26 Q1 PoC → 2026.06 V2 → V6 固定顺序链路（Stage0-5 每步留 artifact 可回验）
- 数字：对比表 2天+→~5分钟；内容生成 天级→~3分钟；文献综述 天级→~3分钟；Source Fidelity 100% / FN 0% / FP ~12% / 对齐 >95%；3 份 CT CER 进入 NMPA 递交流程
- 素材源（在 cer-global-share-speech 仓库）：
  - deck/0509_CER_Automation_Deck.html（主 Deck，v4/v6 为历史版本）
  - materials/CER_LLM_Layer_Architecture_20260807.html
  - materials/CER_Stage1_Ordered_Alignment_Ribbon_Architecture_Casebook_20260803.html
  - video/scenes/v8/PLAY.html（12 幕分镜）、video/scenes/v2/previews/*.png（截图）
  - ppt/SSME_QT_CER-0618.pptx、ppt/SSME_QT_CER_0509.pptx
  - speech/20260807_全球平台分享演讲稿_主稿12页.md

### Layer 2 · AIDU Strategy（口述整理，名称以实际为准：口述"AIDU"，可能与 AIDO/AIDI 同源，请核实）
- 流程：所有 BU × 各 Function → AIDU Interface Team → 深入组织挖 User Ideas → 评分机制 → 筛选；Fast Win 项目获更多人才流入
- 落地：自提自落（自己提自己落地）/ 自提他落（团队合力解决）
- 资源：① 内部人才库 ② IT 资源 ③ 外部供应商资金与资源
- 叙事定位：CER 项目 = AIDU 机制里的 Fast Win 样板

### Layer 3 · 个人职业发展
- 一句话定位：在 SSME 框架下做"把 AI 落进真实合规业务"的人
- 四幕主线 / 三个方法论标签（业务驱动、边界感、工程化落地）/ 成长线 RA→AIPO、本地 AIDO→全球 AIDI
- 素材：career-portfolio/01-叙事框架-高管对话.md、02-口播稿-3分钟版.md（本仓库外，可让 Jianan 提供或直接引用内容）

### Layer 4 · 潜在答疑（5 问）
- Q1 老板最关注 QT 什么指标 / Q2 QT AI 自动化往哪落地 / Q3 组织 AI talent 前景 / Q4 对我这样年轻人的指引 / Q5 对年轻人的建议
- 每问带"为什么问这个"（展示思考深度）

## 3. 设计约束

- 风格对齐本仓库 index.html 的 Apple Minimal 暗色系（#0B0B0F 背景、渐变色强调、等宽字体标注）
- 保持单文件自包含优先（内联 CSS；素材嵌入用相对路径指向 cer-global-share-speech 仓库的本地 clone，如 ../../cer-global-share-speech/deck/0509_CER_Automation_Deck.html）
- 中英双语 i18n 可选（index.html 已有 assets/i18n.js 模式可参考）
- 不要破坏 index.html 现有站点结构；新增内容都放 exec-talk/

## 4. Codex 待办清单

1. 把 CER 素材真正嵌入（Deck HTML iframe/截图、LLM 架构图、Stage1 Casebook、v8 PLAY.html 或 v2 previews 截图）
2. AIDU 流程做成动效/更好看的流程图（当前是文字 box 流）
3. 口播稿收录（文本折叠或音频占位）
4. Q&A 卡片样式细化（可切换"只看问题/看为什么"）
5. 可选：发布 GitHub Pages 方便现场手机打开
6. 预留位：Jianan 后续提供最新 PPT/截图后替换 ⏳

## 5. 脱敏注意

- 内部汇报场景（高管 1v1）可保留公司内部指标；若未来对外发布，需去掉：NMPA 递交状态、内部迭代指标、BU 代号（CT/AT/XP/MI）、组织内部名（SSME/AIDU 等视发布范围）
- 发布前过一遍：真实姓名可保留（个人主页），但项目代号/仓库内部链接视范围

## 6. 完成标准

- 单文件 HTML 在浏览器直接打开可完整演示四层
- 每层有可视化（CER 数字卡+素材嵌入、AIDU 流程、个人主线、Q&A）
- 无外部依赖断链（本地 clone 路径正确）
- git commit 到 Jianan-Career-Pathway 并 push
