# 训练营配套 Skill 生产规范（yuanskill-pro 纪律，所有生产者必读必守）

## 最高原则
**课稿是唯一内容源，不自行发挥。** 每条规则、公式、步骤、数字、示例必须出自：
1. 课稿原文：`~/creator-camp-skill-mining/feishu-doc.md`（各自简报给了行号范围）
2. 反馈文档定稿规格：简报中已逐字引用
3. 既有 sm-* skill 中「已标注源自课稿」的部分（可继承其 references 逐字提取）

无法溯源到以上三处的内容**不写**；确需推导性示例的，逐条标 ⚪（待人工核实）。

## 目录与文件（每个 skill）
```
<skill-name>/
  SKILL.md          # 正文 ≤100 行（不含 frontmatter）
  references/       # 课稿逐字提取 + 模板，只允许一层引用
  evals/eval.md     # 检查项 + ≥1 正例 + ≥1 易混反例 + 基线对比结论
  CHANGELOG.md      # 变化清单：每个组成部分标来源（课稿第X节 / 反馈规格 / 继承sm-xx / ⚪推导）
```

## SKILL.md 字段级工程
- frontmatter：`name`（=目录名，kebab）+ `description`（触发公式：何时用 + 用户会怎么说的触发词 + 不适用边界，中文，一段写完）
- 触发条件只写在 description，正文不重复
- 正文用中文；三层渐进披露：description → 正文流程 → references 细节
- 正文必须写明「何时读哪个 reference 文件」，只放不提=白放
- 约束分三层：**铁律**（源自课程红线，违反即输出无效）/ 写作规范 / 踩坑点

## 课程红线（所有 skill 通用，各自按课稿措辞落地）
- 真实性：无真实记录/数据不生成事实句；AI 不凭想象编造体验、数据、案例
- 对外承诺、报价、评分排名：AI 出草稿，人拍板
- 前后对比要公平；不伪造在场细节

## 评测（yuanskill-pro 阶段 7，不可省略）
在你自己的上下文里做基线对比：取 evals 里的正例输入，(a) 不看 SKILL.md 直接答一遍；(b) 严格按 SKILL.md 流程答一遍。对照客观检查项给两者打分，把记分与结论写进 `evals/eval.md`。反例要选**容易混淆的**（如：对种草 skill 用「帮我写条测评」）。

## 其他
- 不改本工作区其他 skill 目录；不改课稿快照与 sm-* 原件
- 中文正文；代码/目录/文件名英文
- 语气与格式对齐范例：`~/.claude/skills/sm-tutorial-script/SKILL.md`
