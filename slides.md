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

一场有效的内部分享不仅包含选取合适的内容，内容的呈现方式、分享内容的后续利用都有助于让一场准备充分的分享价值最大化。

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

# 📃 分享目的


---
layout: two-cols
---
# 准备分享内容上的几点优先诉求

- 利用率
  - 团队当下或未来是否会使用此分享内容
  - 是否解决了团队当下的某个问题
  - 是否适用于参会的大多数人
- 通俗易懂
  - 明确面向的群体，使用特定的语言
  - 使用类比描述晦涩难懂的事物
  - 适当地重复表达重要内容
- 问题解决
  - 当下团队面临的主要问题（一个或几个）
  - 个人面对并解决了的问题

::right::

<img class="h-100 m-10" src="https://cdn.pixabay.com/photo/2019/06/25/08/09/priority-4297708_1280.jpg">


---
layout: two-cols
---

# 额外目的

1. 形成良好的团队习惯
2. 利于展开下一个阶段工作
3. 满足公司与团队的学习型组织要求


::right::

<img src="https://cdn.pixabay.com/photo/2016/03/28/14/19/destination-1285851_1280.png">


---
layout: center
---

### 👇 案例

[《文字与格式》分享](文字与格式.pdf)

<br>
<br>

<img class="h-80" src="https://cdn.pixabay.com/photo/2015/02/03/23/41/paper-623167_1280.jpg">


---
layout: center
---

# 📚 **内容转化**

---
layout: two-cols
---

# 转化率

- 优先关联性
  - 与团队最近的发生的事情产生关联
  - 与下个阶段的工作产生关联
- 提升利用率
  - 文档先行，分享结束后以可执行文档影响团队后续工作
  - 成功经验先行，以成功的案例作为分享核心
- 分享及时性

::right::

<br>
<br>

<img class="h-90" src="https://cdn.pixabay.com/photo/2018/08/18/13/27/browser-3614768_1280.png">


---
layout: center
---

# 💡 分享模式

---
layout: two-cols
---

# 模式分类

- PPT 讲述
- 动态画图
- 发散讲解
- 文档式

::right::

<img src="https://cdn.pixabay.com/photo/2021/11/24/11/58/coach-6820960_1280.jpg">

---
layout: center
---

# ⌨️ 质量保障

---
layout: two-cols
---

# 内容质量

- 确保内容有效和当前正确性
- 宁缺毋滥、以身作则
- 前期指导 + 纠正与迭代

::right::

<img class="m-5" src="https://epicwebtechno.com/wp-content/uploads/2019/02/uu.jpg">


---
layout: center
---

# Q&A
