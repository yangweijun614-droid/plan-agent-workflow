---
name: plan-agent-workflow
description: Use when designing a small AI agent workflow and deciding its steps, tool inputs and outputs, dependencies, or stopping conditions. 适用于设计 Agent 工作流。
---

# Agent 工作流拆分

把用户目标改写成可检查的交付物。为每个步骤写清输入、动作、输出和完成条件。列出上一步产物是下一步前提的位置，再标出可以独立进行的步骤。

把固定计算交给普通代码，把需要理解文本或根据中间结果做判断的步骤交给模型。为循环设置退出条件，为缺数据和工具失败写出处理方式。遇到对外发送或修改记录等操作时，在流程里写明所需授权和完成后要核对的结果。

示例：做文档问答时，流程可以是读取问题、检索片段、基于片段作答。没有足够证据时，终止并说明缺哪些材料。交付物是一段带可核对来源的答案。
