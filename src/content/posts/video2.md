---
title: 在帖子中嵌入视频2
published: 2025-01-18
description: 这篇文章演示了如何在博客文章中包含嵌入视频。
image: "./img/a (1).jpg"
tags: [HTML,视频]
category: 示例
draft: false
---

:::note
采用HTML5内制播放器+R2对象存储桶实现
:::

```yaml

本地视频源：<video width="300" height="500" src="https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E8%A7%86%E9%A2%91/%E5%A4%A9%E7%A9%B9.mp4" controls="controls"></video>

```

# 采用 `video标签`
```yaml
<video width="720" height="1280" src="https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E8%A7%86%E9%A2%91/%E5%A4%A9%E7%A9%B9.mp4" controls="controls"  controlsList="nodownload" disablePictureInPicture autoplay loop ></video>
```
<video width="720" height="1280" src="https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E8%A7%86%E9%A2%91/%E5%A4%A9%E7%A9%B9.mp4" controls="controls"  controlsList="nodownload" disablePictureInPicture autoplay loop ></video>

# 控件删减
- 1.去掉画中画和下载功能
```yaml
controlsList="nodownload"  disablePictureInPicture
```
![](https://img2020.cnblogs.com/blog/1105185/202112/1105185-20211231113447413-1725646922.png)

>参考：`https://www.cnblogs.com/carriezhao/p/15752031.html`

- 2.自动播放 `autoplay` 和 循环播放 `loop`
```yaml
<video width="" height="" src=""  controlsList="nodownload" disablePictureInPicture autoplay loop ></video>
```
