---
title: 在帖子中嵌入视频2
published: 2025-01-18
description: 这篇文章演示了如何在博客文章中包含嵌入视频。
tags: [示例,视频]
category: 示例
draft: false
---

自制播放器+R2对象存储桶实现

```yaml
---
title: 在帖子中包含视频2
published: 2025-01-18
// ...
---
Bilibili：<iframe width="100%" height="468" src="//player.bilibili.com/player.html?bvid=BV1fK4y1s7Qf&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
YouTube：<iframe width="100%" height="468" src="https://www.youtube.com/embed/5gIf0_xpFPI?si=N1WTorLKL0uwLsU_" title="YouTube video player" frameborder="0" allowfullscreen></iframe>
本地视频源：<video width="300" height="500" src="https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E8%A7%86%E9%A2%91/%E5%A4%A9%E7%A9%B9.mp4" controls="controls"></video>

```

>## 自制播放器+R2对象存储桶实现
<video width="720" height="970" src="https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E8%A7%86%E9%A2%91/%E5%A4%A9%E7%A9%B9.mp4" controls="controls"></video>
