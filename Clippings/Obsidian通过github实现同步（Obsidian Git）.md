---
title: "Obsidian通过github实现同步（Obsidian Git）"
source: "https://zhuanlan.zhihu.com/p/657924375"
author:
  - "[[残差不收敛怎么办现在在一个冷门且炎热的国家念书ing～]]"
published:
created: 2026-03-17
description: "感觉是最快最方便的实现同步的方法了。整套操作下来如果顺利五分钟就可以搞定~而且一劳永逸╰(*°▽°*)╯ 文章末尾有俺滴碎碎念... 功能实现本文包含配置Github的步骤，Github新手友好。所以文科小姐姐也可以轻松…"
tags:
  - "clippings"
---
目录

收起

功能实现

Obsidian端

Github

碎碎念

![](https://pica.zhimg.com/v2-0fab4c76a11ac116f092fb6b7ce32d8e_1440w.jpg)

记得勾选private

发布于 2023-09-23 03:57・沙特阿拉伯[GitHub](https://www.zhihu.com/topic/19566035)[Obsidian](https://www.zhihu.com/topic/21349840)[同步- remotely save- obsidian git](https://www.zhihu.com/topic/26483364)[多知识任务还在排队做？腾讯ima同步处理省时间](https://ima.qq.com/download/?webFrom=10000435&channel=10000435&cb=https%3A%2F%2Fsugar.zhihu.com%2Fplutus_adreaper_callback%3Fsi%3D79f1a7ea-f135-43c9-96a5-63f08f9c2ffb%26os%3D3%26zid%3D1629%26zaid%3D3665261%26zcid%3D3621071%26cid%3D3621071%26event%3D__EVENTTYPE__%26value%3D__EVENTVALUE__%26ts%3D__TIMESTAMP__%26cts%3D__TS__%26mh%3D__MEMBERHASHID__%26adv%3D703838%26ocg%3D4%26cp%3D2500%26ocs%3D1%26aic%3D0%26atp%3D0%26ct%3D2%26ed%3DGiBNJgVzfCMmUW9XIVDVNQZREwA%3D&spu=biz%3D0%26ci%3D3621071%26si%3D0e3983f0-3f01-4661-9985-d5d1230b70ce%26ts%3D1773740119%26zid%3D1629)

[

微信文件一键转存至腾讯ima知识库，让你想用的时候随时都能用，还能对知识库里的文件进行深层次解析哦

](https://ima.qq.com/download/?webFrom=10000435&channel=10000435&cb=https%3A%2F%2Fsugar.zhihu.com%2Fplutus_adreaper_callback%3Fsi%3D79f1a7ea-f135-43c9-96a5-63f08f9c2ffb%26os%3D3%26zid%3D1629%26zaid%3D3665261%26zcid%3D3621071%26cid%3D3621071%26event%3D__EVENTTYPE__%26value%3D__EVENTVALUE__%26ts%3D__TIMESTAMP__%26cts%3D__TS__%26mh%3D__MEMBERHASHID__%26adv%3D703838%26ocg%3D4%26cp%3D2500%26ocs%3D1%26aic%3D0%26atp%3D0%26ct%3D2%26ed%3DGiBNJgVzfCMmUW9XIVDVNQZREwA%3D&spu=biz%3D0%26ci%3D3621071%26si%3D0e3983f0-3f01-4661-9985-d5d1230b70ce%26ts%3D1773740119%26zid%3D1629)