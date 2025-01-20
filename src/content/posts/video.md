---
title: 在帖子中嵌入视频
published: 2023-08-01
description: 这篇文章演示了如何在博客文章中包含嵌入视频。
tags: [示例,视频]
category: 示例
draft: false
---

只需从 Bilibili、YouTube或其他平台复制嵌入代码，并将其粘贴到 markdown 文件中即可。

```yaml
---
title: 在帖子中包含视频
published: 2023-10-19
// ...
---
Bilibili：<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=928861104&bvid=BV1uT4y1P7CX&cid=287639008&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
YouTube：<iframe width="100%" height="468" src="https://www.youtube.com/embed/5gIf0_xpFPI?si=N1WTorLKL0uwLsU_" title="YouTube video player" frameborder="0" allowfullscreen></iframe>
```

>## Bilibili
<iframe width="100%" height="468" src="//player.bilibili.com/player.html?isOutside=true&aid=928861104&bvid=BV1uT4y1P7CX&cid=287639008&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

>## YouTube
<iframe width="100%" height="468" src="https://www.youtube.com/embed/5gIf0_xpFPI?si=N1WTorLKL0uwLsU_" title="YouTube video player" frameborder="0" allowfullscreen></iframe>