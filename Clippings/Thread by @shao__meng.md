---
title: "Thread by @shao__meng"
source: "https://x.com/shao__meng/status/2034063363588657275"
author:
  - "[[@shao__meng]]"
published: 2026-03-18
created: 2026-03-22
description:
tags:
  - "clippings"
---
**meng shao** @shao\_\_meng 2026-03-17

如何打造高效 Claude Code Skills —— 来自 Claude Code 开发者 Thariq 数百个 Skills 的真实经验总结

Thariq 帮我们系统梳理了 Skills 的本质、分类、最佳实践及分发策略，强调 Skills 并非“仅 Markdown 文件”，而是可包含脚本、资产、数据的文件夹，并支持动态钩子等高级配置。

Skills 的核心定义与价值

Skills 让 AI Agents 能“发现、探索并操纵”特定领域知识与工具，形成可复用、可组合的“技能包”。最大价值在于：

· 解决 AI Agents 默认知识的局限（内部库、设计规范、业务流程等）

· 通过文件系统实现“渐进式披露”，让上下文工程更高效

· 支持内存存储（日志/JSON/SQLite）、脚本复用、按需钩子，实现真正“智能”而非死板执行

九大 Skills 类型（内部实践分类）

1\. 库与 API 参考：提供内部/常用库的正确用法、代码片段、gotchas（陷阱）。示例：billing-lib、frontend-design

2\. 产品验证：集成 Playwright、tmux 等工具，确保输出正确。建议投入工程师一周时间打磨。示例：signup-flow-driver、checkout-verifier

3\. 数据获取与分析：连接监控/数据栈，包含查询模式、凭证。示例：funnel-query、grafana

4\. 业务流程自动化：一键完成重复工作，支持日志记忆。示例：standup-post、weekly-recap

5\. 代码脚手架与模板：生成带业务规范的 boilerplate。示例：new-migration、create-app

6\. 代码质量与评审：自动审查、风格强制、可集成 GitHub Action。示例：adversarial-review

7\. CI/CD 与部署：监控 PR、渐进 rollout、回滚。示例：babysit-pr、deploy-<service>

8\. Runbooks：症状→多工具诊断→结构化报告。示例：oncall-runner、log-correlator

9\. 基础设施运维：含防护栏的破坏性操作。示例：orphans-cleanup、cost-investigation

制作 Skills 的核心技巧

· 不陈述显而易见：聚焦 AI Agents 默认认知之外的信息（如设计品味、内部 footguns）

· 构建 Gotchas 专区：持续迭代，记录 AI Agents 常见失败点——这是最高价值内容

· 利用文件系统：文件夹即上下文；拆分 references/api.md、assets/template.md，实现渐进披露

· 避免过度约束：给灵活性，让 AI Agents 适应场景

· Setup 与内存：用 config.json 存用户配置；日志/数据库实现自记忆（稳定路径用 ${CLAUDE\_PLUGIN\_DATA}）

· 脚本优先：提供 helper 函数库，让 AI Agents 专注组合而非重写 boilerplate

· 按需钩子：如 /careful 阻塞危险命令，仅在必要时激活。

描述字段技巧：写给模型看的“触发条件”，而非用户摘要

分发与管理策略

· 内部：检入仓库（./.claude/skills）或自建 Plugin Marketplace

· 市场化：有机生长 + PR 审核，避免冗余；用 PreToolUse 钩子追踪使用率

· 组合：Skills 可互相引用，实现依赖链

· 公共/开源：目前市场化尚不完善

> 2026-03-17
> 
> ![图像](https://pbs.twimg.com/media/HDpx0XLbEAEkCWA?format=jpg&name=large) ![文章封面图片](https://pbs.twimg.com/media/HDl2jn9a0AAZkyz?format=jpg&name=large)