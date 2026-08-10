# HANDOVER · 高管 1v1 四层对话材料包

> 仓库：`Jianan-Huang0609/Jianan-Career-Pathway`
> 目录：`exec-talk/`
> 基线：`05bb4f1`（2026-08-10 生成前）
> 本轮交付：`01-四层材料包.md`、`02-高管对话-展示.html`、`03-HANDOVER-codex.md`
> 未修改：`00-原材料-原始需求.md`、`04-HANDOVER-PROMPT.md`

---

## 1. 交付目标

这套材料服务于 Jianan 与公司高管的内部 1v1，不是公开简历，也不是纯技术汇报。它用四层结构串联：

```text
CER 真实成果
   ↓
AIDU Strategy（口述整理，名称待核实）的组织机制理解
   ↓
RA → AI Product 的个人成长线
   ↓
围绕 QT、AI talent 与年轻人成长的方向校准
```

核心叙事：**在 SSME 框架下，做“把 AI 落进真实合规业务”的人。**

---

## 2. 三个交付物分别做什么

### `01-四层材料包.md`

- 完整四层材料总集，可用于备稿、核数与后续持续更新。
- 包含 CER 历程、四块能力、数据与人机边界。
- AIDU Strategy 每个关键位置均标注“口述整理，名称待核实”。
- 收录 Jianan 原始需求与 3 分钟口播底稿。
- 每个拟向高管提出的问题均附“为什么问这个”。
- 单列素材清单、历史版本差异与统一预留位。

### `02-高管对话-展示.html`

- 单文件、自包含；浏览器直接打开，不依赖网络或同级仓库资源。
- 四层可视化分别是：
  1. CER 时间轴、数字锚点、四能力与人机边界；
  2. AIDU Strategy（口述整理，名称待核实）五步机制流、两种落地模式、三类资源；
  3. RA → AI Product 成长阶梯与三个方法论标签；
  4. QT / AI talent / 年轻人成长提问矩阵。
- 内联交互：阅读进度、问法理由展开、素材路径复制。
- 无障碍：语义化结构、跳转链接、键盘焦点、`aria-expanded` / `aria-live`、`prefers-reduced-motion`。
- 打印：`@media print` 转白底、展开问法理由、隐藏导航与交互控件。

### `03-HANDOVER-codex.md`

- 记录真源、取舍、设计合同、维护边界、验证方式和待办。

---

## 3. 已读取素材与使用方式

以下素材路径相对于 `/Users/jianan/.openclaw/workspace`。

| 素材 | 读取结果 | 主要用于 |
|---|---|---|
| `repos/Jianan-Career-Pathway/exec-talk/00-原材料-原始需求.md` | 已完整读取 | 原始需求、四层框架、AIDU 口述逻辑、提问方向 |
| `repos/Jianan-Career-Pathway/exec-talk/04-HANDOVER-PROMPT.md` | 已完整读取 | 交付结构、指定数字、内容与设计约束 |
| `agents/sam/career-portfolio/01-叙事框架-高管对话.md` | 已完整读取 | 一句话定位、四幕主线、方法论、质量与效率指标 |
| `agents/sam/career-portfolio/02-口播稿-3分钟版.md` | 已完整读取 | 口播主线、人机边界与高管追问回答 |
| `repos/cer-global-share-speech/deck/0509_CER_Automation_Deck.html` | 已读取相关页面和数据 | 四块能力、产品化叙事、3 分钟历史展示口径、质量指标 |
| `repos/cer-global-share-speech/materials/CER_LLM_Layer_Architecture_20260807.html` | 已读取 | Stage00–5、Gate、artifact、人审回路、API 与 Analysis Chat |
| `repos/cer-global-share-speech/materials/CER_Stage1_Ordered_Alignment_Ribbon_Architecture_Casebook_20260803.html` | 已读取 | Stage1 有界语义、exact evidence、owner、编译与发布边界 |
| `repos/cer-global-share-speech/video/scenes/v8/PLAY.html` | 已读取 | 播放器结构与场景注册状态 |
| `repos/cer-global-share-speech/video/scenes/v2/previews/*.png` | 已盘点 | 历史视觉参考；未嵌入 HTML |
| `repos/cer-global-share-speech/ppt/SSME_QT_CER-0618.pptx` | 11 页已逐页提取文本，并渲染为全页预览检查 | FY26 成果、协作、路线与指标 |
| `repos/cer-global-share-speech/speech/20260807_全球平台分享演讲稿_主稿12页.md` | 已完整读取 | 业务背景、四功能、边界、团队与下一步 |

### 素材未直接嵌入的原因

任务同时要求“引用现有材料”和“HTML 单文件自包含、无外部依赖”。因此展示页采用：

- 把已核验内容转成页面内可视化；
- 在素材索引中保留精确路径与复制按钮；
- 不使用跨仓库 iframe、外部图片、外链字体或外部脚本。

这样即使只复制 `02-高管对话-展示.html`，现场仍可完整打开。若以后要把真实 Deck 或截图嵌入单文件，应使用经过脱敏与授权的压缩后 base64 资源，并留意文件体积。

---

## 4. 数字与版本口径

### 本轮高管对话采用

- PoC：**FY26 Q1**
- V2：**2026.06**
- V6：**Stage0–5 固定链路**
- 对比表：**2 天以上 → 约 5 分钟**
- 内容生成与文献综述：**天级 → 约 3 分钟**
- Source Fidelity：**100%**
- False Negative：**0%**
- False Positive：**约 12%**
- 列间对齐：**>95%**
- 业务采用：**3 份 CT CER 进入 NMPA 递交流程**
- 下一步：Multi-BU、PDF 多格式、Analysis Chat、能力 API 化

### 已发现的历史材料差异

1. **对比表耗时**
   - 本任务和 career-portfolio：`2 天以上 → 约 5 分钟`；
   - 0509 主 Deck：页面写 `3 Min`。
   本轮按任务指定采用“约 5 分钟”。如果现场打开 0509 Deck，应按该历史页面原文解释，不要把两个数字说成同一轮测试。

2. **PoC 时间**
   - 本任务和 0618 PPTX：`FY26 Q1`；
   - 0509 主 Deck 历史时间线：`2025 Q3`。
   本轮按任务指定采用 `FY26 Q1`。

3. **Stage 粒度**
   - 高管口径：`Stage0–5`；
   - 2026-08 技术材料：`Stage00 + Stage0–5`。
   这是叙事粒度不同。高管对话不主动展开 Stage00，除非对方追问技术架构。

4. **V8 场景数**
   - `video/scenes/v8/` 中存在 12 个 `scene-*.html`；
   - 当前 `PLAY.html` 的 `scenes` 数组只注册前 7 个。
   在播放器修复前，应说“目录有 12 幕素材，当前播放器可导航前 7 幕”，不要直接说“播放器已支持 12 幕”。

---

## 5. AIDU Strategy（口述整理，名称待核实）边界

硬性规则：

- 每个标题、流程图、核心叙事或正式提问中出现 AIDU 时，补充 **“口述整理，名称待核实”**。
- 可以说明它“可能与 AIDO / AIDI 等同源”，但不能自行确认。
- CER 只能表述为 **Fast Win 候选样板** 或“按我的理解可作为样板”，不能声称已被该机制正式认定。
- 待正式名称、owner、评分机制与 Interface Team 核实后，再统一改名；不要只改标题而漏掉正文、无障碍标签或打印内容。

---

## 6. 展示页设计合同

### 视觉方向

- 基底：`#0B0B0F`。
- 风格：暗色 Apple Minimal，但采用“高管 briefing dossier”而非通用 dashboard。
- 识别线：单一橙色 `#FF6A2A` 作为证据与进度信号；薄荷色用于已验证/人的控制权；琥珀色用于名称或边界提醒。
- 标题：本地宋体栈，形成编辑感；标签和数字：系统等宽字体；正文：Avenir / 中文无衬线本地栈。
- 版式：大标题、克制卡片、宽留白、细分隔线；不用外部字体、图标库或装饰图片。

### 交互与可访问性

- 问题卡的“为什么问”由按钮控制，状态通过 `aria-expanded` 暴露。
- 剪贴板失败时给出 `aria-live` 文本反馈，不让功能静默失败。
- 尊重 `prefers-reduced-motion`。
- 打印时强制显示所有“为什么问”，避免纸面缺失信息。

### 维护原则

- 不添加 CDN、外链字体、远端 JS 或必须联网的资源。
- 数字更新时，同步检查 CER 指标卡、补充口径、应答条和来源差异说明。
- AIDU Strategy（口述整理，名称待核实）的正式名称更新时，全局搜索 `AIDU`、`AIDO`、`AIDI` 与 `名称待核实`。
- 面向公开个人网站之前，必须另做公开版，不直接复用内部版。

---

## 7. 脱敏与发布边界

本轮按“公司内部 1v1”保留任务明确允许的内部指标。禁止直接公开发布前，至少重新审查：

- NMPA 递交状态与产品范围；
- CT / XP / AT 等 BU 代号；
- SSME、AIDU Strategy（口述整理，名称待核实）等组织或机制名；
- 内部路线图、资源与时间点；
- 源仓库路径、技术架构与截图；
- 真实用户反馈、人员与团队信息。

本材料没有写求职状态，也没有加入任务以外的个人隐私。

---

## 8. 验证方式

在仓库根目录运行：

```bash
git diff --check
rg -n "第 1 层|第 2 层|第 3 层|第 4 层|⏳ 预留位，待补充" exec-talk/01-四层材料包.md
rg -n "id=\"cer\"|id=\"aidu\"|id=\"career\"|id=\"questions\"|@media print|prefers-reduced-motion" exec-talk/02-高管对话-展示.html
rg -n "https?://|<link|<iframe|<img|src=\"//" exec-talk/02-高管对话-展示.html
rg -n "AIDU" exec-talk/01-四层材料包.md exec-talk/02-高管对话-展示.html exec-talk/03-HANDOVER-codex.md
git diff -- exec-talk/01-四层材料包.md exec-talk/02-高管对话-展示.html exec-talk/03-HANDOVER-codex.md
```

预期：

- 四层结构、预留位、打印与减弱动效规则均命中；
- 外链依赖检查不应命中 `http(s)`、`<link>`、`<iframe>`、`<img>` 或协议相对脚本；
- AIDU Strategy（口述整理，名称待核实）的关键出现位置保留完整标注或明确指向同一警示；
- `git diff --check` 无空白错误；
- Git 只包含 01 / 02 / 03 三个目标文件的变更。

---

## 9. 下一步待办

### 会前必须确认

- [ ] AIDU Strategy（口述整理，名称待核实）的正式名称；在核实前保持完整标注。
- [ ] 选择现场只问的 2–3 个问题，不要逐题照读。
- [ ] 确认 3 份 CT CER 的最新内部口径没有变化。
- [ ] 用目标会议设备离线打开 HTML，并测试打印或 PDF 备份。
- [ ] 如果要播放 V8，先补齐 `PLAY.html` 后 5 幕导航或只演示前 7 幕。

### 会后回流

- [ ] 记录高管最关注的 QT 指标。
- [ ] 记录对 AI talent 与 RA → AI Product 的具体建议。
- [ ] 把行动项写成 owner / date / evidence，而不是只留感想。
- [ ] 将新材料填回 `01-四层材料包.md` 的预留位。

### 未来公开版

- [ ] 单独建立 public-safe 数据口径与脱敏清单。
- [ ] 将内部仓库路径替换为经授权的作品集摘要。
- [ ] 个人网站按履历 / 能力 / 作品集 / 项目经历分区，但保留“证据来源”和“我的具体贡献”。

---

## 10. 交付状态

本文件与 `01-四层材料包.md`、`02-高管对话-展示.html` 应在同一提交中交付。提交信息使用 Conventional Commits：

```text
feat(exec-talk): refine executive conversation package
```

最终提交 hash 与 push 结果以本次执行报告和仓库 `git log -1` 为准。
