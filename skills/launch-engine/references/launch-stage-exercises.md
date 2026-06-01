# Launch阶段练习详细指南

## 练习1：创始人瓶颈审计

**原版Exercise**：Use Claude Cowork to run a structured audit of your current operational load, documenting every recurring task, every decision that lands on your desk, and every workflow that only happens because you personally remember to do it.

**执行方法**：
1. 花1小时记录过去一周你做的每一件事（不要遗漏小事）
2. 按以下维度分类：
   - 只有你能做的（战略决策、关键客户、融资）
   - 需要人但不需要你的（日常运营、客服、报告）
   - 可以完全自动化的（数据同步、文档更新、定时任务）
3. 计算你花在"只有你能做"的事情上的时间比例
   - <30%：你在做正确的事
   - 30-60%：有优化空间
   - >60%：你是瓶颈

## 练习2：消失测试

**原版Exercise**：Ask Claude to extrapolate what happens to each workflow when you're unavailable for a week.

**执行方法**：
1. 假设你下周完全不可用
2. 逐个工作流问：没有我会怎样？
3. 会停滞的工作流 = 你的瓶颈
4. 为每个瓶颈设计替代方案：
   - 文档化（让别人能接手）
   - 自动化（让AI代替）
   - 委托（交给团队成员）

## 练习3：技术债偿还排期

**原版Exercise**：Direct Claude Code to audit your MVP codebase and produce a prioritized list. Then feed that list to Claude and ask it to sequence the remediation work.

**执行方法**：
1. Claude Code做代码审计：结构弱点、测试覆盖缺口、重构候选
2. 把审计结果给Claude排序：什么必须现在修、什么可以和功能开发并行、什么可以等
3. 关键：把MVP期间存在于你脑子里的架构决策写入CLAUDE.md

## 练习4：合规差距分析

**原版Exercise**：Run a code-level security review with Claude Code oriented to the frameworks your target market requires.

**执行方法**：
1. 确定目标市场需要的合规框架（SOC 2, GDPR, HIPAA等）
2. Claude Code做代码级安全审查
3. Claude帮你排优先级和设计控制措施
4. 把合规工作流融入开发周期，而非一次性项目
5. 为企业买家准备合规文档

## 练习5：产品管理流程

**原版Exercise**：Ask Claude to design a lightweight product management operating system.

**执行方法**：
1. 设计轻量产品管理体系：
   - Sprint节奏
   - 最低规格的spec模板
   - Bug分诊决策树
   - 周度指标简报
2. 用Claude Cowork运行运营层：排期、路由、报告编译
3. 目标：流程不需要你触发就能运转

## 练习6：怀疑论者审视

**原版Exercise**：Ask Claude to make the adversarial case against your own traction.

**执行方法**：
1. 把你的增长数据交给AI
2. 要求AI扮演怀疑论者，找出数据中最弱的环节
3. 问：这些数字最可能的替代解释是什么？
4. 问：如果增长是假的，它会怎么伪装成真的？
5. 对每个怀疑论论点，要求事实证据回应，不接受"我觉得"
