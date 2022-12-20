---
title: "1219 Loveit"
subtitle: ""
author: ""
date: 2022-12-19T18:28:17+08:00
lastmod: 2022-12-19T18:28:17+08:00
draft: false
description: ""
images: []

tags: []
categories: []

twemoji: false
---
### 实现功能

#### 一、`Katex` 公式编辑及渲染

1. 这是行内公式：

    $x^2 + y^2 + z^2 = \frac{e^{xy}}{3\pi}$
2. 段落公式：
   
   $$\cos^3x + 2\cos2x\sin3x = \sin^3x$$

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
   
