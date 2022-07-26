---
# try also 'default' to start simple
theme: seriph
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

# 项目的局部重构

流程分享

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# 什么是局部重构?

面对项目中无法解决、改动风险大等种类的问题，由研发团队发起的代码局部改造工作。通过代码的结构变化、业务设计、性能调优等方面的变化，最终解决团队问题。

- 📝 **目的性** - 明确重构的目的，以解决问题作为重构的发起原因，以最终问题是否解决衡量重构的好坏
- 🎨 **方案制定** - 制定明确、详细、可衡量的技术方案
- 🧑‍💻 **风险评估** - 明确重构所带来的风险，要对可能发生的风险做到把控
- 🤹 **资源消耗与收益** - 明确重构所付出的资源（研发工时、测试工时等）与所带来的回报
- 🕐 **时间规划** - 制定详尽的时间规划表，用于推进重构按部就班进行，提高最终的结果交付率
- 📚 **过程记录** - 对整个重构过程中的关键节点、关键事件做到完整记录
- 🛠 **项目复盘** - 开发完成并上线后对整个重构过程进行复盘

<br>
<br>

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

# 局部重构流程

对于客户端研发团队的局部重构，需要按照以下流程进行。 [learn more]()

### 环节 内容

|     |     |
| --- | --- |
| 内容发起| 由个人或团队发现问题，并进行重构行为的发起。 |
| 项目评审 | 针对发起的内容（需有初版方案），由团队负责人进行项目评审 |
| 方案讨论与制定 | 团队负责人参与进行方案讨论与制定 |
| 项目开发与推进 | 由发起人（项目负责人）主导重构内容开发与进度把控 |
| 过程记录与汇报 | 由发起人（项目负责人）进行整个重构过程的记录 |
| 项目复盘 | 开发完成并上线后，由发起人（项目负责人）对整个重构过程进行复盘 |

根据以上所有内容，组装成一个完整的项目文档。
---

# 示例 -- SN 业务解耦

以 SN 业务解耦为示例，进行一个完整重构内容的展示。 [^1]

### 目的性
SN 是目前系统中对于货品管理过程中的核心业务功能，嵌入到了系统各类业务模块（出入库、箱子、退货等）中。伴随着此模块的业务需求增加（强化弱序列号功能、B2B 模块未来的变化、医药行业对于 SN 的管控），对于此模块的修改愈发频繁。因之前代码设计的原因，所带来的就是更改业务过程中容易出现以下几个问题。

- 现在的原因
  - 对于问题或业务的修改容易出现遗漏
  - 同一功能嵌入不同业务，测试需全部业务核验，无法仅做一次核验
- 未来的原因
  - 新人去修改业务时无法全局思考，只能针对需求做机械式更改
  - 代码冗余原因、导致很难全局检查业务不一致性

针对以上问题，个人觉得有必要对 SN 模块进行局部代码重构，解决以上问题的发生。

[^1]: [SN 业务解耦项目文档]()
---

# 示例 -- SN 业务解耦

<div grid="~ cols-2 gap-4">
<div>

### 方案制定

#### 1、风险评估

#### 2、资源消耗与收益

</div>
<div>

#### 3、时间规划

|  **时间范围**   |  **预期内容**  |
| --- | --- |
| xx年xx月xx日 -- yy 日 | 完成重构方案设计 |
| xx年xx月xx日 -- yy 日 | 完成所有关于 SN 功能的业务梳理，明确业务影响范围 |
| xx年xx月xx日 -- yy 日 | 代码结构搭建已完成。目前进度为项目整体的 30%。 |

</div>
</div>

---
layout: two-cols
---

# 示例 -- SN 业务解耦

### 过程记录

|  **时间范围**   |  **关键动作**  |
| --- | --- |
| xx年xx月xx日 -- yy 日 | 完成重构方案设计 |
| xx年xx月xx日 -- yy 日 | 完成所有关于 SN 功能的业务梳理，明确业务影响范围 |
| xx年xx月xx日 -- yy 日 | 代码结构搭建已完成。目前进度为项目整体的 30%。 |

::right::

<img class="m-5" src="https://llv.edu.vn/media/2022/03/process.jpg">

---
class: px-20
---
# 注意事项

对于整个的重构过程可能出现的问题提一些建议。

<div grid="~ cols-2 gap-4">
<div>

- 进度阶段性汇报
- 注意时间进度的偏移程度
- 理解项目文档的重要性
- 重视初版方案与 DEMO 制作
- 重试沟通与表达

</div>
<div>

<img class="m-5" src="https://austinkleon.com/wp-content/uploads/2012/10/00-show-cover.jpg">

</div>
</div>


---
layout: center
class: text-center
---

# Learn More

[系统局部重构的规则与流程]() · [SN 业务解耦项目文档]() 

---
layout: center
---

# Q&A