---
title: 关于Astro添加背景音乐的问题
published: 2025-01-19
description: 记录Astro添加背景音乐的问题
image: "./img/天穹.jpg"
tags: [Astro,背景音乐]
category: 示例
draft: false
---

<!-- TOC -->
* [观察Astro项目结构](#观察astro项目结构)
* [想办法在主页添加音乐](#想办法在主页添加音乐)
<!-- TOC -->

# 观察Astro项目结构
```
├── src/
│   ├── components/    # 可复用的组件
│   │   └── Navigation.astro
│   └── pages/        # 页面文件
│       ├── index.astro
│       └── about.astro
├── public/          # 静态资源
│   └── favicon.svg
├── astro.config.mjs # Astro 配置文件
├── package.json     # 项目依赖配置
└── tsconfig.json    # TypeScript 配置

```

# 想办法在主页添加音乐
- 主页代码名：`[...page].astro`,源代码：
```yaml
  export const getStaticPaths = (async ({ paginate }) => {
  const allBlogPosts = await getSortedPosts()
return paginate(allBlogPosts, { pageSize: PAGE_SIZE })
}) satisfies GetStaticPaths
  // https://github.com/withastro/astro/issues/6507#issuecomment-1489916992

  const { page } = Astro.props

  const len = page.data.length
---

  <MainGridLayout>
//在这里面添加代码成功
  <PostPage page={page}></PostPage>
<Pagination class="mx-auto onload-animation" page={page} style=`animation-delay: calc(var(--content-delay) + ${(len)*50}ms)`></Pagination>
  </MainGridLayout>
```
- 添加音乐播放代码
```yaml
<audio autoplay>
  <source src="" type="audio/mp3">
</audio>
```
- 音乐控件参考菜鸟教程：https://www.runoob.com/?s=audio
> 参考了：[Astro 入门教程](https://juejin.cn/post/7445956009564700726)

