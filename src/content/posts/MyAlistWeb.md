---
title: 关于我的Alist网页端部署
published: 2025-01-28
description: 没钱买服务器，so？
image: "https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E5%8D%9A%E5%AE%A2%E5%B8%96%E5%AD%90%E5%9B%BE%E7%89%87/PixPin_2025-01-29_03-46-00.png"
tags: [说明,Alist]
category: 说明
draft: false
---

- Alist-Web伪展示：https://alist-web-teg.pages.dev

实际只是调用官方api作为成品，我给它套个web壳子，关键代码就是这个：
```yaml
    <script>
      window.ALIST = {
    cdn: undefined,
    monaco_cdn: undefined,
    base_path: undefined,
    api: undefined,  //填入自己的alist网址
    main_color: undefined,
}
      window.__dynamic_base__ = window.ALIST.cdn || ""
      </script>
```
- 参考链接：https://github.com/AlistGo/alist/discussions/6680#discussioncomment-9942683
- 这才是我的真实Alist：
![](https://pub-932bcf23b7c54bdf90743ac393af13cd.r2.dev/%E5%8D%9A%E5%AE%A2%E5%B8%96%E5%AD%90%E5%9B%BE%E7%89%87/screencapture-192-168-135-213-5244-2025-01-29-03_37_22.png)