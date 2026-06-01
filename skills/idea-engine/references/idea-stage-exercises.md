# Idea阶段练习详细指南

## 练习1：问题假设锐化

**原版Exercise**：Work with Claude to sharpen your problem statement until it's a testable hypothesis.

**执行方法**：
1. 写下你的问题陈述（1-2句话）
2. 对照可测试性标准逐项检查：
   - 能否说出谁有这个问题？（不能只说"大家"）
   - 能否说多久发生一次？（不能只说"经常"）
   - 能否说多严重？（需要量化：时间/金钱/机会）
   - 能否说他们现在怎么应对？（"没有方案"通常是假信号）
3. 每个不可测试的部分，追问一个层次

**迭代示例**：
- 第1轮："人们报销很痛苦" → 不可测试
- 第2轮："员工填报销单很烦" → 还是不够具体
- 第3轮："中型公司的财务经理每周花4+小时核对报销，因为工具和会计软件不集成" → 可测试

## 练习2：魔鬼代言人

**原版Exercise**：Ask Claude to argue against your idea, and to find disconfirming evidence that refutes your hypothesis.

**执行方法**：
1. 把你的完整假设（问题+方案方向）交给AI
2. 要求AI输出：
   - 3-5条最强反面论证
   - 失败的类似产品案例
   - 市场结构性的不利因素
3. 不要反驳AI的反面论证——先全部记录
4. 然后逐条评估：哪些反面论证有事实支撑？哪些基于假设？
5. 有事实支撑的反面论证必须回应，不能忽略

**关键原则**：AI follows your direction。如果你问"这个想法有什么问题"，AI会找到问题。如果你问"帮我看看这个想法行不行"，AI倾向于支持你。措辞很重要。

## 练习3：竞品分层映射

**原版Exercise**：Ask Claude to map your competitive landscape by tier: direct competitors, indirect competitors, potential acquirers, and adjacent players.

**执行方法**：
1. 逐层搜索，不要一次性全列
2. 每层至少找3个实体
3. 对每个竞品，回答："为什么这个对手可能赢而我不会？"
4. 特别注意第四层（相邻玩家）——最大的威胁往往来自你没注意到的地方
5. 如果四层都很稀疏，要么是你发现了真正的蓝海（罕见），要么是你没找够（常见）

**Competitor Neglect检查**：
- 你是否系统性地低估了竞争对手的威胁？
- "没有竞争"更可能是你的搜索盲区，而非市场空白

## 练习4：用户访谈问题审计

**原版Exercise**：Draft your interview questions by hand first, ask Claude to audit them.

**执行方法**：
1. 先手写访谈问题（不要让AI生成——自己写的过程本身就是思考）
2. 让AI审计，检查：
   - 面向未来的问题（"你会用吗？"）→ 改为面向过去（"上次遇到时你怎么做的？"）
   - 引导性问题（"你觉得X功能有用吗？"）→ 改为开放式（"跟我说说你上次处理X的经历"）
   - 社交期望问题（"你觉得这个重要吗？"）→ 改为行为问题（"你上次为此花了多少时间？"）
3. 为关键问题设计2-3个追问探针

**核心原则**：问过去的行为，不问未来的意愿。人们预测自己行为的准确率极低。

## 练习5：访谈后信号分析

**原版Exercise**：After every five interviews, direct Claude Cowork to synthesize your notes and produce two lists.

**执行方法**：
1. 每做完5个访谈，整理所有笔记
2. 提取两份清单：支持假设的证据 vs 挑战假设的证据
3. 每条证据必须引用具体访谈（不能只说"有人提到"）
4. 如果支持清单显著长于挑战清单，追问：这种不对称是数据本身，还是你想找到的东西？
5. 标记所有"你可能选择性地解读了信号"的位置

**信号质量评估**：
- 行为证据（用户实际做了什么）> 态度证据（用户说了什么）
- 过去行为 > 未来承诺
- 具体描述 > 模糊赞同

## 练习6：方案概念最终检查

**原版Exercise**：Present your solution concept to Claude and ask it to identify the three assumptions your design depends on most heavily.

**执行方法**：
1. 写下你的完整方案概念
2. 识别方案最依赖的3个假设
3. 对每个假设回答：
   - 什么条件下这个假设成立？
   - 如果不成立，后果是什么？
4. 确认方案解决的是验证发现的问题，不是最初假设的问题

## 练习7：轻量原型

**原版Exercise**：Define the single core interaction your solution depends on. Direct Claude Code to build only that.

**执行方法**：
1. 只定义一个核心交互——不是完整产品，是验证用的道具
2. 用Claude Code构建最小可用原型
3. 放到5个验证过的目标用户面前
4. 观察：他们能用吗？他们的反应是什么？他们想回来再用吗？
5. 这5次对话决定：继续构建还是回到画板
