# 🤖 HANDOVER PROMPT — 高管对话四层框架材料生成

> 这是可直接复制给 Agent（Codex / Claude / 任何 coding agent）的 prompt。
> 用法：把下面【HANDOVER PROMPT 开始 → 结束】之间的内容整段复制，丢给你的 agent。
> 原材料已整理在同目录 `00-原材料-原始需求.md`；本 prompt 已自包含（不依赖该文件也能跑）。

---

## HANDOVER PROMPT 开始

你是 Jianan 的素材整理助手。Jianan 下周要和公司高管 1v1 聊自己的职业发展与成果，请你按他指定的**四层框架**生成一份完整的高管对话材料包，并写回 GitHub 仓库 `Jianan-Career-Pathway` 的 `exec-talk/` 目录。

## 背景（原始需求）

Jianan 原话："我下周需要和公司的一个高管稍微聊一下我自己，主要方向是讲述我在 SSME 的框架下做了什么事情，表现出我比较优秀的点可以串起来。新建一个 GitHub，以后职业发展、更新简历都可以往这个方向聚合，包括搭建自己的个人网站——履历/能力/作品集/项目经历等等板块。"

## 四层框架（必须严格按此结构生成）

### 第 1 层 · CER 材料
- 把 CER 的现有 HTML 材料直接附上/引用（素材路径见下）
- 简要介绍历程与关键节点（PoC FY26 Q1 → V2 2026.06 → V6 固定链路 Stage0-5；四块能力：提取填充/Comparison/Difference Analysis/Literature Review；量化结果：对比表 2天+→~5分钟、内容生成与文献综述 天级→~3分钟、Source Fidelity 100%、FN 0%、FP ~12%、对齐 >95%；3 份 CT CER 进入 NMPA 递交流程；下一步 Multi-BU/PDF 多格式/Analysis Chat/API 化）
- 预留位：Jianan 后续会再给材料，先标注"⏳ 预留位，待补充"

### 第 2 层 · AIDU Strategy
- 按以下逻辑整理（口述，名称待核实——"AIDU"可能为 AIDO/AIDI 等同源，需在文档中标注）：
  ① 聚合所有 BU 和各 Function → ② 形成 AIDU Interface Team → ③ Interface 深入组织内部挖掘 User Ideas → ④ 评分机制筛选 → ⑤ Fast Win 项目获更多人才流入
- 落地两模式：自提自落（自己提自己落地）/ 自提他落（团队合力解决）
- 资源三来源：① 公司内部人才库 ② IT 资源 ③ 外部供应商的钱和资源
- 叙事定位：CER 项目 = AIDU 机制里的 Fast Win 样板

### 第 3 层 · 个人职业发展
- 把 Jianan 之前的提示词原文拎出来作为基础材料包（见本 prompt 开头"背景"段的原话，以及仓库 `00-原材料-原始需求.md` 全文）
- 加上现有 HTML/口播稿作为底料（素材路径见下）
- 叙事核心：在 SSME 框架下做"把 AI 落进真实合规业务"的人；RA → AI Product 成长线；三个方法论标签（业务驱动/边界感/工程化落地）

### 第 4 层 · 潜在答疑
按三个提问方向生成问题清单，每题附"为什么问这个"：
1. 对 QT 方向：作为老板最关注 QT 的什么指标？想把 QT 的 AI 自动化往什么方向落地？
2. 对组织内 AI talent：发展前景和能力建设如何？对年轻人（我）有没有指引方向？（含我自己的职业发展困惑）
3. 对潜在的答疑和给年轻人的建议

## 素材路径（读取这些文件做底料）

- `agents/sam/career-portfolio/01-叙事框架-高管对话.md`、`02-口播稿-3分钟版.md`
- `repos/cer-global-share-speech/deck/0509_CER_Automation_Deck.html`（主 Deck，v4/v6 历史版）
- `repos/cer-global-share-speech/materials/CER_LLM_Layer_Architecture_20260807.html`
- `repos/cer-global-share-speech/materials/CER_Stage1_Ordered_Alignment_Ribbon_Architecture_Casebook_20260803.html`
- `repos/cer-global-share-speech/video/scenes/v8/PLAY.html`（12 幕分镜）、`video/scenes/v2/previews/*.png`（截图）
- `repos/cer-global-share-speech/ppt/SSME_QT_CER-0618.pptx`、`speech/20260807_全球平台分享演讲稿_主稿12页.md`

（以上路径相对于 `/Users/jianan/.openclaw/workspace`；若 agent 无法访问某文件，跳过并在结果中注明即可，不要编造数据。）

## 交付物（写回 `repos/Jianan-Career-Pathway/exec-talk/`）

1. `01-四层材料包.md` — 四层框架的完整材料总集（结构：总览 → CER → AIDU → 个人发展 → 答疑 → 素材清单 → 预留位）
2. `02-高管对话-展示.html` — 单文件自包含 HTML 展示页（暗色 Apple Minimal 风格：`#0B0B0F` 背景、卡片式布局、等宽字体标注；四层分区，数字高亮；浏览器直接打开可用，无外部依赖）
3. `03-HANDOVER-codex.md` — 交接文档（说明素材源、设计约束、待办）
4. git commit + push 到 `Jianan-Huang0609/Jianan-Career-Pathway`

## 约束

- 全中文（人名/专有名词除外）
- 脱敏：内部指标可保留（内部 1v1 场景）；不写真实姓名以外的隐私；不暴露招聘/求职状态
- 数据只来自素材文件，不编造数字；拿不到就标注"待补充"
- AIDU 名称必须标注"口述整理，名称待核实"

## 完成标准

- 四层框架齐全、每层有可视化表达
- 展示 HTML 可直接打开演示
- 已 push，给出 commit hash

## HANDOVER PROMPT 结束
