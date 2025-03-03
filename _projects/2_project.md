---
layout: page
title: LAN
description: 横板动作射击游戏
img: assets/img/3.jpg
importance: 2
category: Group
giscus_comments: true
---

主要负责玩法设计、前两关关卡设计以及怪物AI射击。

玩家将控制一个机械生物，从初始形态开始，逐步通过挑战性的关卡。在游戏过程中，你将获得三种独特的子弹能力，每种能力都带来新的游戏机制。

游戏融合了经典平台跳跃元素与创新的射击玩法，玩家需要策略性地利用四种子弹的独特属性，克服每个关卡的挑战。

<!-- 添加视频链接 -->
<strong style="font-size: 24px;">视频演示</strong>
<p>点击下面的链接查看视频演示：</p>
<a href="https://www.bilibili.com/video/BV1tw9iYdEor/" target="_blank" class="btn btn-primary">点击观看视频</a>

<strong style="font-size: 24px;">游戏玩法</strong>

<strong style="font-size: 20px;">1. 玩家行为</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/玩家行为.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

1. 分为基本行为和射击行为

2. 基本行为包括基本移动、跳跃、攀墙跳以及墙壁抓取

3. 射击行为随着关卡进程会逐步获取，包括攻击子弹、重力子弹、反弹子弹、磁力子弹

<strong style="font-size: 20px;">2. 核心玩法循环</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/核心玩法循环.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

1. 分为基本行为和射击行为

2. 基本行为包括基本移动、跳跃、攀墙跳以及墙壁抓取

3. 射击行为随着关卡进程会逐步获取，包括攻击子弹、重力子弹、反弹子弹、磁力子弹

<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
