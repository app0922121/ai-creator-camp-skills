# CHANGELOG · social-account-doctor-course

## v1.0.0（2026-08-17）初版

Based on JuneYaooo/social-account-doctor (MIT)。上游 LICENSE 已拷贝为 `references/UPSTREAM-LICENSE`。

### 组成部分与来源

| 组成部分 | 来源 |
|---|---|
| 核心改造「拆爆款→拆账号」：近约 20 条 / 聚类高频选题而非只看最高赞 / 主页商业承接 / 代表性内容评论区提问 / 标明实际取得条数与覆盖范围（铁律 1-3、第 0 步、第 2 步③） | 课程组反馈定稿第 1 点 |
| 三类对标 + 头腰尾组合（第 1 步） | 课稿第三节「找 3 类对标账号」（561-723 行），逐字见 references/course-benchmark.md 第二节 |
| 五处拆解（第 2 步表格） | 课稿第三节「拆对标账号的 5 个位置」，逐字见 references/course-benchmark.md 第三节 |
| 四项判断（需求信号/具体问题/信任形式/变现承接）、"验证判断"命名、事实/推断/未知三分法（铁律 4、第 3 步） | 课程组反馈定稿第 2 点；四维度原文出自课稿（references/course-benchmark.md 第四节） |
| 评论区需求聚类六字段（第 2 步④） | 课程组反馈定稿第 3 点 |
| 主页四件套：昵称 3 版 / 三行简介 3 版 / 置顶 3 条 / 前 10 条栏目（第 4 步） | 课程组反馈定稿第 4 点；四件套原文出自课稿（references/course-homepage.md 第二节），"3 版供拍板"结构继承 sm-homepage |
| 主页示意图轻量模板 assets/homepage-mockup-template.html（手机框+头像位+简介三行+九宫格，抖音/小红书双主题，不装 html-anything/归藏卡片） | 课程组反馈定稿第 4 点 + 课稿呈现形式说明；⚪ 占位符命名、双主题配色、前 3 格置顶角标等实现细节为工程推导 |
| 铁律 1「数据必须真实喂入，禁止凭账号名想象」、铁律 2「不硬凑 20 条」 | 课程组反馈定稿铁律（课程红线：幻觉高发） |
| 铁律 5「对标不是抄爆款/跟风」 | 课稿原文（references/course-benchmark.md 第一节） |
| 铁律 6 前半（资历数字不虚构） | CONVENTIONS 课程通用红线 + 继承 sm-homepage 边界 |
| 铁律 6 后半（报告面向非技术用户）、数据覆盖标注（半成品显式标注）、tikhub CLI 代抓公开数据可选路径、接口失败回退用户粘贴 | 继承上游 JuneYaooo/social-account-doctor（H6 / H3 / §7 工具速查 / find Step 3 兜底） |
| 数据收集清单（references/course-benchmark.md 第六节） | ⚪ 继承 sm-benchmark 同名推导清单（非课稿原文，已标注） |
| 「学不学归用户拍板」「多账号逐个拆+横向对照」边界 | 继承 sm-benchmark 边界 |
| evals/eval.md 正例虚构测试数据 | ⚪ 评测用 fixture，已在文内标注非真实账号 |

### 相对上游的删改

- 删：find/crack/adapt/compose/commerce 全命令体系、诊断模式、评分词表、平台阈值表、scripts/ 与 tikhub/ 目录（课程版不携带代码，只在数据获取处引用本机已装的上游 CLI 作可选路径）。
- 改：产出从「下一条可发笔记初稿」改为「账号级验证判断 + 主页装修四件套 + 示意图」；「验证结论」改为「验证判断」。
- 留：真实数据铁律、完整度标注、⚪/事实标注习惯、非技术用户报告语言、接口失败透明兜底。

### 基线评测

见 evals/eval.md：裸答 2.5/10 vs 按 skill 10/10，结论有效。
