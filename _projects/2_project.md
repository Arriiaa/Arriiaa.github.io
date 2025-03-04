---
layout: page
title: LAN
description: 2D平台射击游戏
img: assets/img/3.jpg
importance: 2
category: Group
giscus_comments: false
---

主要负责玩法设计、前两关关卡设计以及怪物AI设计。

玩家将控制一个机械生物，从初始形态开始，逐步通过挑战性的关卡。在游戏过程中，你将获得三种独特的子弹能力，每种能力都带来新的游戏机制。

游戏融合了经典平台跳跃元素与创新的射击玩法，玩家需要策略性地利用四种子弹的独特属性，克服每个关卡的挑战。

<!-- 添加视频链接 -->
<strong style="font-size: 24px;">视频演示</strong>
<p>点击下面的链接查看视频演示：</p>
<a href="https://www.bilibili.com/video/BV1444y1k7Ci/" target="_blank" class="btn btn-primary">点击观看视频</a>

<strong style="font-size: 24px;">游戏玩法</strong>

<strong style="font-size: 20px;">1. 玩家行为</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/玩家行为.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    玩家行为总览
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/move.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/jump.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/扒住墙.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    跑、跳、墙壁抓取
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/蹬墙跳-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/蹬墙跳-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/蹬墙跳-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    攀墙跳
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/重力2-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/重力2-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/重力2-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    重力子弹
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/反冲1-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/反冲1-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    反冲子弹
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/磁力2-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/磁力2-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    磁力子弹
</div>

1. 分为基本行为和射击行为

2. 基本行为包括基本移动、跳跃、攀墙跳以及墙壁抓取

3. 射击行为随着关卡进程会逐步获取，包括攻击子弹、重力子弹、反弹子弹、磁力子弹

<strong style="font-size: 20px;">2. 特殊设计：人抢分离</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/人枪分离.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

在设计初期，我们选择了玩家持枪攻击的方式。然而，在进行整合时，由于枪支需要跟随鼠标，当玩家持枪时会出现许多问题，例如：
   
   ① 玩家需要360°射击，如果玩家持枪，角色会不停旋转，导致移动不流畅；
   
   ② 手臂与墙壁之间的角度也会在使用磁性子弹时造成问题。

因此，我们采用了人枪分离设计，将枪支完全与角色分开。

另外，我们发现，由于枪支跟随玩家，二者之间会存在相对距离，这会导致子弹的射击位置和反馈功能与玩家之间存在一定的差异，要求玩家自行判断。这种设计方式将增加游戏的策略性和可玩性。

<strong style="font-size: 20px;">3. 核心玩法循环</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/核心玩法循环.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

1. 共有两个循环，外层循环和内层循环

2. 外层循环为整个游戏的循环系统，内层循环为一个关卡内部的循环系统

<strong style="font-size: 24px;">游戏叙事</strong>

<strong style="font-size: 20px;">1. 世界观</strong>

科技已经远比当今发达，人们可以用意识接入网络，又或者通过放生科技制造替代身体部位 义肢甚至活生生的人;国家接近形同虚设，大型企业的触角则遍布社会各个角落，社会贫富 也因此更加差距悬殊;底层群体彻底成为边缘人群，生活看不到未来和希望，即便有反抗也 会被消解。

<strong style="font-size: 20px;">2. 主线流程</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/主线流程.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<strong style="font-size: 20px;">3. 核心体验</strong>

动作带来的成就感和爽快感: 玩家在游戏过程中会感受到使用各种子弹翻越障碍物，击败敌人，闯过一个个小关卡的成就感和流畅的游戏操作、较低的死亡惩罚给玩家带来的爽快感。

<strong style="font-size: 24px;">怪物设计</strong>

<strong style="font-size: 20px;">1. 小怪设计</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/小怪类型.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/怪物AI.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

1. 共有三种小怪，近战、远程以及移动病毒，前两者基本逻辑相似，仅为攻击范围以及攻击角度不同。

2. 由于项目比起动作游戏来说更偏向于平台游戏，因此小怪在该项目中的重要性低于相关障碍物。甚至移动病毒更偏向于障碍物而非小怪。

<strong style="font-size: 20px;">2. BOSS设计</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS AI.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    BOSS AI设计
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS Q.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    BOSS美术设计
</div>

1. 想尽量将BOSS的AI做的复杂一些，让玩家在最后的时候将情绪递到最高

2. 在设计过程中还是吃了没有经验的亏，设计出来后，试玩体验较差，但由于项目时间问题，只能做出些微的修改。希望下次在做设计的时候能够多迭代几次。

<strong style="font-size: 24px;">关卡设计</strong>

<strong style="font-size: 20px;">1. 关卡元素</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡元素.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<strong style="font-size: 20px;">2. 关卡平面图</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡设计1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    第一关平面图
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡设计2-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    第二关平面图前半段
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡设计2-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    第二关平面图后半段
</div>

<strong style="font-size: 20px;">3. 关卡展示</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡1-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡1-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    关卡一
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡2-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡2-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    关卡二
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡3-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡3-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    关卡三
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡4-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡4-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    关卡四
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡5-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/关卡5-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    关卡五
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS-4.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/BOSS-5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    BOSS关卡
</div>

最初由于缺乏经验，我们这样设计关卡：脑暴机关，根据大概难度感知组合机关。

几乎必然的结果就是，关卡难度梯度模糊，且新内容缺乏逐步地引导。因此重构时，我们将所有的机关、需要玩家习得的技能，分成平台类、机关障碍类、移动类三个维度，根据学习的子弹作用分析当前关卡所偏重的模块、引入的新机制，并根据小怪的数量来调节难度，从而一定程度做到对难度梯度和节奏游戏节奏的控制。

<strong style="font-size: 24px;">美术设计</strong>

<strong style="font-size: 20px;">1. 角色设计</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/夏娃.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/丹尼尔.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<strong style="font-size: 20px;">2. 场景及UI设计</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/场景.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    场景设计
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/book_covers/登陆界面.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    登陆界面
</div>
