# AI 创作者商业化训练营 · 配套 Agent Skills

《AI 创作者商业化训练营》课程官方配套技能包。**课稿是唯一内容源**：每个 skill 的规则、公式、步骤、示范均逐字取自课程原文（存于各 skill 的 `references/`），结构按课程组反馈文档定稿规格实现，推导性内容一律标 ⚪。

## 技能清单（7 个）

| Skill | 对应课程 | 一句话 |
|---|---|---|
| [ai-creator-positioning-workbench](ai-creator-positioning-workbench/) | 第二课 · 定位 | 访谈式定位工作台：九步流程 20–30 分钟产出《AI 账号定位卡》并写入《账号毕业档案》，AI 不替学员定案 |
| [social-account-doctor-course](social-account-doctor-course/) | 第三课 · 对标拆解 | 拆账号（非拆爆款）：近 20 条聚类 + 三类对标 + 五处拆解 + 四项验证判断（事实/推断/未知）+ 主页装修四件套与模拟图 |
| [tutorial-script-sixgrid](tutorial-script-sixgrid/) | 第五课 · 教程脚本 | 复现六格教程脚本初稿：真实任务记录强制输入，无记录不生成，可拿走资产人验证后才发 |
| [review-test-orchestrator](review-test-orchestrator/) | 第六课 · 测评脚本 | 测评执行编排：同任务同标准 ×3 重复 + 证据对比表，「最看重 X 则选 Y」逐条挂证据行号，无实测不出评分排名 |
| [seeding-script-generator](seeding-script-generator/) | 第八课 · 信任种草 | 四锚点种草脚本成稿 + 内置发布前逐环自检（零伪造成本空话标注），在场细节必须真实 |
| [purchase-decision-copywriter](purchase-decision-copywriter/) | 第九课 · 购买决策 | 四账逐笔算（时间/金钱/确定性/身份，强制有数字有推理）+ 三闸收口，数字与承诺人工核实 |
| [zhijia-deal-pricing](zhijia-deal-pricing/) | 第12课 · 品牌商单 | 智价·商单报价测算：Brief 确认表（十项防漏，授权/排他必问）+ 底价公式 + 三档方案，最终报价人拍板 |

## 安装

```bash
# 全部安装（Claude Code 全局）
cp -R <skill-name> ~/.claude/skills/<skill-name>

# 或只装单个，装完新开会话生效
```

每个 skill 自包含：`SKILL.md`（≤100 行正文）+ `references/`（课稿逐字提取）+ `evals/`（检查项与基线对比记录）+ `CHANGELOG.md`（逐组件来源溯源）。

## 通用红线（全部源自课程）

- **真实性**：无真实记录/数据不生成事实句，AI 不凭想象编造体验、数据、案例
- **对外动作人拍板**：报价、评分排名、发布承诺——AI 出草稿与测算，人做决定
- **前后对比要公平**，不伪造在场细节

## 生产方式与许可

- 生产流程：yuanskill-pro（需求解构 → 形态判定 → 定义可验证标准 → 合成 → 基线评测）。每个 skill 都做过「裸跑 vs 按 skill」基线对比，记分见各 `evals/eval.md`
- 结构规格来源：课程组反馈文档（2026-08-17 定稿）；内容来源：课稿 2026-08-12 快照
- `social-account-doctor-course` 基于 [JuneYaooo/social-account-doctor](https://github.com/JuneYaooo/social-account-doctor)（MIT）定制，上游许可见其 `references/UPSTREAM-LICENSE`
- 其余内容为《AI 创作者商业化训练营》课程资产，版权归课程方所有，未经许可请勿转载分发
