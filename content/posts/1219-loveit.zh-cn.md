---
title: "实现功能汇总"
subtitle: ""
author: ""
date: 2022-12-19T18:28:23+08:00
lastmod: 2022-12-19T18:28:23+08:00
draft: false
description: ""
images: []

tags: []
categories: []

twemoji: true
password: 123xxaxx321
---
{{< music auto="https://music.163.com/#/playlist?id=60198" loop="auto">}}

* [X] 实现功能

#### **基本功能使用说明**

1. 文章优先发布在中文环境下的 `posts`，可以根据内容建立相应文件夹，主要命令如下：

```markdown
hugo new posts/new.zh-cn.md
```

2. 对于部分文章，可选加密功能 `password`
3. 设置合理 `tags` 进行归档管理
4. `assets/images` 用来存储插图，可以直接引用就能渲染,或者直接存储在 `content/posts` 下，在 `.md` 中进行直接调用，还有可以直接调用，具体方法如下：

   {{< image src="/images/1671431328440.png" caption="Lighthouse (`另一种插入图片方法`)" >}}

#### 一、`Katex` 公式编辑及渲染

1. 这是行内公式：

   $x^2 + y^2 + z^2 = \frac{e^{xy}}{3\pi}$
2. 段落公式：

   $$
   \cos^3x + 2\cos2x\sin3x = \sin^3x
   $$

#### 二、`Emoji` 表情

常见表情有：可爱捏😄、笑死我了😂、爱你😘

#### 三、`giscus` 评论

主要在 `github` 中引入该功能，需要开通 `discussion`，同时按要求配置基本信息

#### 四、自定义 `custom style`

主要加入了最新文章统计、根据需要设定 `Font` 和格式

#### 五、加入 `search` 功能

通过配置 `layouts/partials/assets.html` 实现对中文分词并搜索，需要说明的是，该功能需要在 `zh-cn` 环境中使用，同时支持英文搜索功能。因此默认配置可选中文环境。

#### 六、其他功能

1. 支持 music 和 b 站 相关资源在线播放
2. 支持摘要功能
   {{< admonition info >}}
   一个 **信息** 横幅
   {{< /admonition >}}
3. 支持打字机模式 `typeit`
4. 支持语法高亮
5. 支持CDN实现快速渲染
6. 统计浏览量
