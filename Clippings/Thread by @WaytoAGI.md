---
title: "Thread by @WaytoAGI"
source: "https://x.com/WaytoAGI/status/2032397724935692651"
author:
  - "[[@WaytoAGI]]"
published: 2026-03-13
created: 2026-03-17
description:
tags:
  - "clippings"
---
**WaytoAGI｜通往AGI之路** @WaytoAGI [2026-03-13](https://x.com/WaytoAGI/status/2032397724935692651)

10分钟用Obsidian + OpenClaw重构AI知识管理体系👇

我们有幸邀请到了AI自媒体博主@aiwarts 来WaytoAGI分享！他刚完成自己知识体系的完整重构，来分享整套方法。

1️⃣为什么选 Obsidian

Obsidian 的底层是本地 Markdown 文件，AI Agent 直接读写，不需要 API、不需要授权。

Notion、飞书的数据在云端，AI 每次操作都要走 API，慢、贵、有限制，Obsidian 没有这些问题。

2️⃣第一步：统一信息入口

卡尔每天处理五六千条信息，分散在各处。他用三个插件解决入库问题：

飞书文档下载插件 — 批量转成 Markdown 导入

Obsidian Web Clipper — 抓网页，自动保留来源和 tag

微信笔记同步助手 — 微信内容直接同步进来

3️⃣视频和社交平台内容另有方案

X Reader 和 Agent Reach 可以覆盖小红书、公众号、B站、YouTube、抖音、GitHub，连评论区都能抓。

没看过的视频先存链接，确认值得看再用 AI 生成摘要收录，避免无效处理。

4️⃣第二步：搭 AI 能读懂的文件结构

常见误区：把文件夹做得"对人友好"，但 AI 不在乎好不好看，只要路径清晰就够。

推荐起点：GitHub 上有中文版 Obsidian 初始结构项目，包含收件箱、日记、项目研究、知识库、资源管理。卡尔在此基础上加了"工作流存储"目录，放提示词模板和各平台发布 SOP。

看到更好的结构不需要重构，把链接发给 AI，让它把缺少的部分追加进去就行。

5️⃣第三步：用 CodeX 自动维护文件

CodeX 默认绑定目录，直接连接 Obsidian 文件夹，适合管理文件结构。

卡尔每天用它做：整理下载文件夹、批量优化稿件、拆分重组 Markdown、设置定时任务。

分工逻辑：轻量任务先给 CodeX，解决不了交 Claude Code，再解决不了才上 OpenClaw。

6️⃣进阶：用 OpenClaw 让知识库主动运转

OpenClaw 支持心跳机制和 Cron，可以让 Agent 按计划自动扫描知识库、整理新增内容、发送日报，不需要手动触发。

接入方式推荐飞书或 Discord。飞书可以配置多个 OpenClaw 应用共享同一套记忆体系；Discord 有频道隔离，可以在后台同时跑多个任务。

在 OpenClaw 的 agents 配置文件里写清楚哪些内容归到哪个目录，新信息进来就自动分类，不需要二次整理。

7️⃣防止 AI 误操作的两个措施

软链接 — 只开放 Obsidian 特定文件夹的权限，Agent 无法访问其他文件

Git 版本备份 — Code X 在执行命令前后自动存版本，随时可以回退

卡尔的邪修做法：把本地除 Download 文件夹外的所有内容都同步到了 iCloud 2T

8️⃣一个实用细节：上下文健康检测

和 Claude 对话到五六十轮后，它的"遗忘"会明显加速，之前设定的偏好和技能会悄悄丢失。

检测方法：设一个确认指令，能回复关键词说明上下文还在，不行就开新对话。

真正难的不是安装 Obsidian，是想清楚你要管理什么，然后让 AI 读懂你的文件夹逻辑。

#通往AGI之路 #WaytoAGI #OpenClaw #obisidan #claudecode #CodeX #AI知识管理 #知识体系

![图像](https://pbs.twimg.com/media/HDSG9B8a4AEiQoy?format=jpg&name=large) ![图像](https://pbs.twimg.com/media/HDSG9B7bUAAr7X3?format=jpg&name=large) ![图像](https://pbs.twimg.com/media/HDSG9CmaYAEoew8?format=jpg&name=large) ![图像](https://pbs.twimg.com/media/HDSG9B6bwAAp_61?format=jpg&name=large)