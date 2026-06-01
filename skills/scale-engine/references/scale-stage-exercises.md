# Scale阶段练习详细指南

## 练习1：知识外化

**原版Exercise**：Identify one edge case a generic competitor would definitely get wrong in your vertical. Work with Claude Code to build a dedicated test case for it.

**执行方法**：
1. 列出你在这个行业见过的、通用AI一定会搞错的3-5个场景
2. 对每个场景，构建一个测试用例（不是单元测试，是场景测试）
3. 把测试用例加入持续运行的测试套件
4. 每次遇到新edge case就加一条

**关键**：你的测试用例库本身就是护城河地图。它记录了你踩过的所有坑，而新竞争者还没有踩到。

## 练习2：护城河叙事

**原版Exercise**：Ask Claude to help you draft a one-page moat narrative: the story of how your data flywheel works, how long it's been spinning, and why a well-resourced competitor starting today couldn't replicate it in under two years.

**执行方法**：
1. 写一段话（一页纸以内）回答：
   "如果资金雄厚的竞争者今天开始复制你的产品，为什么两年内做不到？"
2. 回答应该包含：
   - 你的数据飞轮怎么运转
   - 它转了多久
   - 时间锁定的数据为什么无法购买或加速
   - 领域知识积累的不可替代性

**注意**：如果你的护城河叙事主要依赖"我们更快"或"我们的AI更好"，那不算护城河。AI是平权的。

## 练习3：Workflow集成深度审计

**原版Exercise**：Ask Claude to help you build a workflow integration audit for your top ten customers.

**执行方法**：
1. 对Top 10客户，逐个记录：
   - 他们构建了哪些自动化
   - 依赖哪些集成
   - 有多少团队工作流通过你的产品
   - 估算迁移成本
2. 找出模式：哪种集成创造最深的锁定？
3. 识别当前在浅层的客户，可以怎么加深

## 练习4：GTM功能构建

**原版Exercise**：Claude builds the product marketing infrastructure.

**执行方法**：
1. Claude协助策略：市场细分、信息架构、分析师关系策略、销售手册
2. Claude Cowork执行运营：内容管道、出站序列、分析师简报、CRM
3. Claude Code构建基建：交互式演示环境、集成文档、沙盒租户、API参考

**关键**：Scale阶段，Loom视频+销售PPT不再够用。买家需要技术评估你的产品。

## 练习5：企业客户差距分析

**原版Exercise**：Pick your three most demanding prospects. Ask Claude to produce a gap analysis.

**执行方法**：
1. 选择3个最理想/最苛刻的目标客户
2. 列出他们采购团队期望看到的一切
3. 对比你的现状，找出差距
4. 排序修复优先级
5. 分配到Claude Code（技术修复）和Claude Cowork（文档/流程）

## 练习6：创始人时间重分配

**原版Exercise**：Use Claude to produce a bottleneck map of your current operational layer. Then ask Claude to extrapolate what happens when you're unavailable for a week.

**执行方法**：
1. 列出只有创始人应该做的事：产品叙事决策、董事会关系、企业大单、创始人间的对话
2. 不在这个列表上的 = 委托或自动化的候选
3. 测试：你消失一周，哪些工作流停滞？
4. 停滞的 = 还需要加强委托/自动化的地方
