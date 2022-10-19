---
# try also 'default' to start simple
theme: default 

# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080

# apply any windi css classes to the current slide
class: 'text-center'

# https://sli.dev/custom/highlighters.html
highlighter: shiki

# show line numbers in code blocks
lineNumbers: false

# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)

# persist drawings in exports and build
drawings:
  persist: false
---

# 如何做一场内部分享

内容与可接受程度的一场妥协？

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# 介绍

一场有效的内部分享不仅包含选取合适的内容，整个内容的呈现方式、分享后续利用都有助于让一场准备充分的分享价值最大化。

在团队内部完成一场内容分享至少要包含或者说需要理清楚以下几个内容。

- 📃 **分享目的** - 如何思考分享行为所带来的的价值。
- 📚 **内容转化** - 如何衡量分享内容是否可转化到实际工作中。
- 💡 **分享模式** - 如何让别人愿意“听”下去。
- ⌨️ **质量保障** - 宁缺毋滥、以身作则。

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: center
---

# 📃 ** 分享目的**

---

## layout: two-cols

# 内部分享的几点优先诉求

- 无歧义
  - 禁止使用反问句
  - 不建议使用表示程度的词汇：**较多、较好、完全地、基本地**
  - 不建议使用表示量的词汇：**有些、非常、大量、一些、少许**
- 通俗易懂
  - 不推荐使用特定人群才了解的词汇
  - 禁止啰嗦冗长、逻辑混乱
  - 勿重复表达同一事物
- 用词恰当
  - [新华社新闻报道中的禁用词（第一批）](https://www.digitaling.com/articles/22975.html)

::right::

<img class="h-100 m-10" src="https://fems.com.au/images/Australian-Standards.jpg">


---

## layout: two-cols

# 额外目的

1. 使用明确使用方式的符号
2. 使用正确中英文格式的符号
3. 禁止使用自造符号：**！！！**

<br>
<br>

👉 [文档格式规范](http://www.zhaowenyu.com/doc-standard/marks.html)
<br>
::right::
<br>
<br>
<br>
<img src="http://www.prcba.com/wp-content/uploads/2020/04/20200425123601_23304.jpg">

---
layout: center
---

# 📚 **内容转化**

---
layout: two-cols
---

# 思考转化率

- 一致性
  - 文档的标点、句式与风格
  - 配图、样式、色彩使用
- 逻辑性
  - 线性逻辑
  - 交叉逻辑
  - 嵌套逻辑
- 学习
  - 基于目的的学习方式
  - 先表面，再深入
  - 以用起来为主

::right::

<br>
<br>
<img class="h-90" src="https://cc-image-resizer.cwg.tw/resize/uri/https%3A%2F%2Fcw1.tw%2FCC%2Fimages%2Farticle%2F201804%2Farticle-5ac1e74a3f09f.jpg/?w=810&h=543&fit=fill">

# 思考转化率

- 一致性
  - 文档的标点、句式与风格
  - 配图、样式、色彩使用
- 逻辑性
  - 线性逻辑
  - 交叉逻辑
  - 嵌套逻辑
- 学习
  - 基于目的的学习方式
  - 先表面，再深入
  - 以用起来为主

::right::

<br>
<br>
<img class="h-90" src="https://cc-image-resizer.cwg.tw/resize/uri/https%3A%2F%2Fcw1.tw%2FCC%2Fimages%2Farticle%2F201804%2Farticle-5ac1e74a3f09f.jpg/?w=810&h=543&fit=fill">

---

layout: center
---

# 💡 **分享模式**

---
layout: two-cols
---

# 目的性的表达

- 场景收集
- 因人而异
  - 软件本地化
  - 语言本地化
- 突出主次

::right::

<img src="https://p3-tt.byteimg.com/origin/dfic-imagehandler/e18d04d7-e693-4118-9f3f-539d43fd37ac">

---
layout: center
---

# ⌨️ **质量保障**

---
layout: two-cols
---

# 案例：[工时设计](https://zsxj.yuque.com/flghe4/hhr1qu/izhpbv)

- 客户端研发源于“目的”进行的需求工时改造
- 采用与之前文档不同的自建模板进行构造
- 整个文档的交付耗时两天
  - 明确内容大纲与呈现方式
  - 填充大纲内容，确保整个内容的全面不遗漏，用文档解释落地制度过程中的所有问题
  - 可被流程图翻译的流程
  - 做错别字、格式一致性、语句通顺与否等基础性检查

::right::

<img class="m-5" src="https://blogimage-1258616042.cos.ap-beijing.myqcloud.com/%E5%9B%A2%E9%98%9F%E5%88%86%E4%BA%AB/%E5%AE%A2%E6%88%B7%E7%AB%AF%E5%B7%A5%E6%97%B6%E8%AE%BE%E8%AE%A1%E4%B8%8E%E9%9C%80%E6%B1%82%E9%A2%86%E5%8F%96%E6%B5%81%E7%A8%8B.jpg">


---
layout: two-cols
---

# 案例：旺店通打印答疑文档

- 面向更大群体的标准化文档
- 对内外均有益的文档
- 能让客户愿意看下去的文档
  - 收集并汇总所有相关问题
  - 填充任何能想到的解决方案
  - 删一半再删一半

::right::

<img class="m-5" src="https://reputationtoday.in/wp-content/uploads/2021/10/learning-doing.jpg">

---

## layout: center

# Q&A
