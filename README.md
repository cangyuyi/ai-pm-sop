# AI PM Resume Writing · AI 产品经理简历写作 Skill

<p align="center">
  <img src="assets/icon.svg" alt="AI PM Resume Writer" width="80" height="80">
</p>

> 给 Codex / AI 编程助手使用的 **AI 产品经理简历写作 SOP 技能**。读完即可独立完成 AI 产品经理（AI 应用/Agent、AI 增长、AI 策略/商业化三个方向）简历的**诊断、撰写与多版本定制**。

## ✨ 能做什么

- 🔍 **简历诊断**：七维度检查（关键词覆盖 / 经历相关性 / 量化充分性 / 证据一致性 / 定位一致性 / 时间线真实性 / 排版扫读友好度），输出匹配度评分、核心优势、改进建议、改写优先级、**面试追问预警**
- 📝 **JD 解析**：三步挖词法（硬技能/软技能/业务场景）+ 词频统计 + JD-证据映射表
- ⛏️ **经历挖掘**：STAR/XYZ 改写，量化 5 法 + 3 种软证据替代，AI 项目六类证据追问
- ✍️ **逐模块撰写**：校招六模块范式，含正反例对照
- 🎯 **多版本定制**：按三大投递方向（AI 应用/Agent / AI 增长 / AI 策略商业化）调整叙事主线
- 📄 **多格式支持**：Markdown、Word (.docx)、PDF、图片截图自动识别

## 🚀 安装

### Codex

将本仓库克隆到 Codex skills 目录：

```bash
git clone https://github.com/cangyuyi/ai-pm-sop.git ~/.codex/skills/ai-pm-resume-writing
```

重启 Codex 或开始新对话后即可自动触发。

### 其他 AI 编程助手（Claude Code / Cursor / Cline 等）

将 SKILL.md 和 references/ 目录复制到你的 Agent 的 instructions/prompts 目录，或将 SKILL.md 内容作为自定义指令的一部分。

## 🎯 使用

直接用自然语言发起即可，例如：

**诊断模式**：
```
这是我的简历[图片/.docx]，帮我看看投 AI 应用方向有什么问题
```

**改写模式（有 JD）**：
```
严格按这份 .docx 模板帮我填内容，版式别动，JD 如下：
[粘贴 JD]
我的经历是：……
```

**通用版（无 JD）**：
```
我还没有目标 JD，先帮我写一份 AI Agent 方向的通用简历，我的经历是……
```

## 📐 核心方法论

### 五条铁律

1. **匹配铁律**：每句话都要回答"这和目标岗位有什么关系"
2. **证据铁律**：每个能力声明必须有经历或数据支撑
3. **量化铁律**：每个结果都要有数字、对比或外部评价
4. **模板铁律**：基于已有简历改写时只改文字不动版式
5. **数据铁律**：不伪造、不篡改、不"合理推测"任何数据

### 三大投递方向

| 方向 | 核心定位 | 最看重的证据 |
|------|----------|-------------|
| **AI 应用/Agent** | 把大模型能力做成可用产品 | Workflow/Prompt 实操、Vibe Coding/MVP、RAG/知识库、评测 SOP、Bad Case 闭环、兜底设计 |
| **AI 增长** | 用 AI + 数据驱动用户增长与转化 | 用户洞察/访谈、内容/渠道实验、私域转化、数据复盘、A/B 测试、增长漏斗 |
| **AI 策略/商业化** | 策略规则设计与商业闭环 | 策略拆解、需求验证、MVP 取舍、定价/交易闭环、收益目标、对照实验思维 |

### AI 项目六类证据

合格的 AI 产品经历必须留下：问题证据、技术选择理由、完整工作流、评测数据、失败案例、迭代结果。仅有"用 Coze 搭了个助手"是不够的。

## 📁 项目结构

```
ai-pm-resume-writing/
├── SKILL.md                    # 入口：工作流程、铁律、模式路由
├── README.md                   # 本文件
├── LICENSE                     # MIT License
├── agents/
│   └── openai.yaml             # Codex UI 元数据
├── assets/
│   ├── icon.svg                # 图标
│   └── resume-template.md      # Markdown 简历输出模板（含填写示例）
└── references/
    ├── capability-and-jd.md    # 能力模型、十大能力族关键词库、JD 解析方法、AI项目六类证据
    ├── mining-and-writing.md   # STAR/XYZ 法则、量化方法、逐模块撰写规范与正反例
    ├── versions-and-diagnosis.md  # 七维度诊断清单、三版本策略、证据缺口补救
    └── redlines-and-checklist.md  # 五条红线、常见误区、成稿自检清单
```

## 🛡️ 安全底线

- **不编造数据**：所有数字必须来自候选人，缺失数据标注 `[待确认]` 而非编造
- **不改原事实**：姓名、学校、公司、时间一字不改
- **不动原版式**：基于 .docx 改写时严格遵循 render-and-verify 流程
- **不替候选人做决定**：有疑点必须追问确认

## 📄 License

MIT License - 详见 [LICENSE](LICENSE) 文件。

## 🙏 致谢

原始 SOP 方法论整理自《AI 产品经理简历写作 SOP 指南》v1.0（2026-08），参考了社区多位 AI 产品面试官与候选人的实战经验。本版本在原始方法论基础上做了 Codex 适配优化（双模式路由、七维度诊断、多格式支持、面试追问预警、渐进式披露等）。
