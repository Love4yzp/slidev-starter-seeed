---
theme: ./theme
title: '演讲标题'
colorSchema: light
transition: slide-left
mdc: true
drawings:
  persist: false
layout: cover
---

# 演讲主标题

<div
  v-click
  transition="duration-500"
  :class="$clicks < 1 ? 'opacity-0 translate-y-2' : 'opacity-70'"
  text-xl mt-2
>
  副标题 · 一句话定位这次分享
</div>

<div v-after flex="~ gap-3" mt-6>
  <SeeedBadge icon="i-carbon:calendar">YYYY.MM.DD · 活动名称</SeeedBadge>
  <SeeedBadge icon="i-carbon:location">深圳</SeeedBadge>
</div>

<div abs-br mx-10 my-8 text-right opacity-40 text-sm>
  [你的名字] · 矽递科技
</div>

<!--
开场白：「今天想和大家分享…」
-->

---
layout: intro
class: pl-30
---

# [你的名字]

<div opacity-75 mt-1 text-lg>
  [你的职位] · 矽递科技 / Seeed Studio
</div>

<div flex="~ gap-2" mt-4 flex-wrap>
  <SeeedBadge>关键词一</SeeedBadge>
  <SeeedBadge>关键词二</SeeedBadge>
  <SeeedBadge>关键词三</SeeedBadge>
</div>

<div my-6 flex="~ col gap-2" text-sm opacity-60>
  <div flex="~ gap-2 items-center">
    <div i-carbon:logo-github text-base />
    <span>github.com/<span style="color: #8FC31F">[你的 GitHub]</span></span>
  </div>
  <div flex="~ gap-2 items-center">
    <div i-carbon:earth text-base />
    <span>[你的网站]</span>
  </div>
</div>

<!-- 头像：放 ./assets/avatar.jpg，不存在时自动隐藏 -->
<img
  :src="'./assets/avatar.jpg'"
  v-click
  absolute top-28 right-20 w-40 rounded-full
  border="2 solid #8FC31F"
  onerror="this.style.display='none'; this.nextElementSibling.style.display='flex'"
/>
<div
  style="display:none"
  absolute top-28 right-20 w-40 h-40 rounded-full
  border="2 dashed gray-300"
  class="flex items-center justify-center text-gray-400 text-xs"
>
  头像
</div>

<!--
自我介绍：一句话带过
-->

---
layout: center
---

「今天想和大家分享两段最近的实践和观察」

<v-clicks>

- [分享点一]
- [分享点二]

</v-clicks>

<!--
谦虚定调：不是来教大家的，是来分享实践的
-->

---

# [问题陈述标题]

> [核心问题一句话]

<v-clicks>

- [问题维度一]
- [问题维度二]
- [为什么现有方案不够好]

</v-clicks>

<!--
「我们团队最近遇到了一个问题…」轻描淡写，不要像在推销
-->

---

# 方案概览

<div class="grid grid-cols-3 gap-4 mt-4">
  <SeeedCard icon="i-carbon:chip" title="[模块一]">
    [模块一的简短描述，一两句话]
  </SeeedCard>
  <SeeedCard icon="i-carbon:cloud" title="[模块二]" color="navy">
    [模块二的简短描述，一两句话]
  </SeeedCard>
  <SeeedCard icon="i-carbon:code" title="[模块三]" color="white">
    [模块三的简短描述，一两句话]
  </SeeedCard>
</div>

<!--
用卡片展示方案的三个核心模块，不要超过三个
-->

---
layout: two-cols-header
leftWidth: 48
---

::header::
# 前后对比

::left::

**之前 (Before)**

- [痛点一]
- [痛点二]
- [痛点三]

::right::

**之后 (After)**

- [改善一]
- [改善二]
- [改善三]

<!--
对比要具体，数字化最好
-->

---

# 系统架构

```mermaid
graph LR
  A["[输入]"] --> B["[处理]"]
  B --> C["[输出]"]
  style A fill:#F0F7DC,stroke:#8FC31F
  style C fill:#F0F7DC,stroke:#8FC31F
```

[替换为实际架构图或 Mermaid 流程图]

<!--
「方案不复杂，核心就是…」简单带一下架构
-->

---
layout: end
---

# 谢谢 · 欢迎交流讨论

<div class="mt-1 text-gray-500 text-sm">
  [你的名字] · 矽递科技 / Seeed Studio
</div>

<div class="flex gap-10 justify-center mt-8">
  <div class="flex flex-col items-center gap-2 group">
    <div class="relative w-28 h-28">
      <img
        :src="'./assets/qr-website.png'"
        class="w-28 h-28 rounded transition-all duration-250 group-hover:opacity-30"
        onerror="this.parentElement.parentElement.style.display='none'"
      />
    </div>
    <span class="text-sm text-gray-500">官网</span>
  </div>

  <div class="flex flex-col items-center gap-2 group">
    <div class="relative w-28 h-28">
      <img
        :src="'./assets/qr-wechat.png'"
        class="w-28 h-28 rounded transition-all duration-250 group-hover:opacity-30"
        onerror="this.parentElement.parentElement.style.display='none'"
      />
    </div>
    <span class="text-sm text-gray-500">微信</span>
  </div>
</div>

<!--
谢谢，开放讨论
-->
