# MVP阶段练习详细指南

## 练习1：架构原则定义

**原版Exercise**：Before opening Claude Code, open Claude and describe what you're building: the core problem it solves, the users it serves, and the scale you realistically expect. Ask it to help you define the architectural principles.

**执行方法**：
1. 不要打开代码编辑器，先打开聊天
2. 描述三件事：
   - 核心问题是什么
   - 服务谁
   - 未来6个月预期的规模（诚实估计，不是梦想）
3. 让AI帮你定义：
   - 架构原则
   - 要避免的依赖
   - 这个阶段主动接受的权衡
4. 保存为CLAUDE.md

**关键**：这个文档是你整个MVP阶段的"宪法"。每个后续session都以它为起点。

## 练习2：Session工作模板

**原版Exercise**：Create a simple session template for your Claude Code work.

**模板**：
```
## Session [日期]
- 目标: [本次session要完成什么]
- 约束: [需要遵守的架构原则/范围限制]
- 上下文: [CLAUDE.md位置]
- 任务: [具体任务描述]

--- session进行中 ---

- 完成: [实际做了什么]
- 决策: [做了什么决策，为什么]
- 假设: [引入了什么假设]
- 技术债: [是否引入技术债，如何记录]
- 下次: [下次session应从哪里开始]
```

**5分钟规则**：每个session结束时花5分钟更新CLAUDE.md的session日志。这5分钟是你对架构漂移最便宜的保险。

## 练习3：安全审查

**原版Exercise**：Before deploying to any real users, run your core application code through Claude with a specific brief.

**审查方向**：
1. 认证与会话管理
2. API响应中的数据暴露
3. 输入验证和注入风险
4. 已知漏洞依赖

**注意**：
- Claude的安全审查是有用的第一轮检查，不是替代
- 涉及认证、密钥、数据处理的事项必须人工审查
- 安全审查应在上线前完成，不是上线后

## 练习4：度量框架预建

**原版Exercise**：Use Claude to define which metrics matter for your specific product, what the benchmarks are, and what patterns in the data would constitute genuine PMF versus flattering noise.

**执行方法**：
1. 在第一个用户出现之前就定义度量框架
2. 确定哪些指标对你的产品有意义
3. 设定Day 1、Day 7、Day 30的基准目标
4. 定义"假阳性"长什么样：注册不激活？付费不留存？初期热情不复用？
5. 当数据到来时，让Claude从怀疑论者角度审视你的数据

**关键**：先定义"什么样的数据说明我错了"，再看数据。否则你会自动找到"数据说明我对了"的角度。

## 练习5：PMF判断

**原版Exercise**：The Sean Ellis test + The effort test.

**Sean Ellis测试**：
- 问活跃用户："如果不能再使用这个产品，你会有多失望？"
- >40%答"非常失望" = 有意义的PMF指标
- 注意样本：必须是活跃用户，不是所有注册用户

**努力曲线测试**：
- PMF前：留存需要你推（频繁触达、激励、跟进）
- PMF后：产品自己拉用户回来
- 从"推"到"拉"的转折点 = PMF真正发生的时刻

**综合判断**：没有任何单一数据点能确认PMF。PMF是一个必须在多个迭代周期中持续存在的模式。
