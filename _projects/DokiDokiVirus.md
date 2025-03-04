---
layout: page
title: DokiDokiVirus
description: 弹幕射击
img: assets/img/DokiDoki.png
importance: 2
category: Group
giscus_comments: false
---

主要负责卡牌系统、部分数值设计

玩家将操控一个可以吞噬敌人的机械生物，在战斗中自由切换吞噬与射击形态，通过不断进化适应挑战性的关卡。

游戏融合了 Roguelike 机制与成长式卡牌升级系统，玩家可选择不同能力强化自身，并利用分裂细胞机制策略性地战斗。

<!-- 添加视频链接 -->
<strong style="font-size: 24px;">视频演示</strong>
<p>点击查看视频演示：</p>
<a href="https://www.youtube.com/watch?v=MMTJhMXP3fU" target="_blank" class="btn btn-primary">点击观看视频</a>

<!-- 添加文档链接 -->
<strong style="font-size: 24px;">英文文档</strong>
<p>点击查看英文文档：</p>
<a href="https://docs.google.com/document/d/1d1qS7FObiesjMkHP4CwzUQmkBtA0QuniCpLt_OdkiEU/edit?tab=t.0" target="_blank" class="btn btn-primary">点击查看文档</a>

<!-- 添加文档链接 -->
<strong style="font-size: 24px;">游玩</strong>
<p>点击进行游玩：</p>
<a href="https://mingx1.itch.io/dokidoki-virus" target="_blank" class="btn btn-primary">点击游玩</a>

<strong style="font-size: 24px;">游戏简介</strong>

《DokiDoki Virus》是一款生存游戏，玩家需要在进攻与防御两种形态之间切换，以对抗不断扩散的病毒。玩家必须在“吞噬”和“射击”两种形态之间策略性地切换，并通过卡牌系统升级能力，以求生存并阻止病毒蔓延至整个屏幕。

<strong style="font-size: 24px;">游戏概述</strong>

《DokiDoki Virus》为玩家提供了一个动态战场，病毒会在屏幕中央不断扩散。玩家必须攻击病毒边缘，吞噬小型敌人，并升级自身能力以求生存。独特的双形态机制增加了策略深度，要求玩家在战斗中平衡进攻与防御。此外，游戏引入了轻度 RPG 元素，玩家可以通过卡牌升级系统提升自身能力。

<strong style="font-size: 24px;">玩家体验</strong>

<strong style="font-size: 20px;">1. 背景与游戏场景</strong>

游戏设定在一个微观环境中，玩家需要对抗迅速扩散的病毒。视觉设计采用暗色调的细胞主题，以增强紧张感和紧迫感。病毒和小型敌人采用明亮的对比色，以引导玩家注意力。随着病毒增长，环境会动态变化，模拟病毒扩散的过程。游戏还包括粒子特效、脉动动画以及病毒边缘的光晕效果，以增强危机感。

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    玩家可以通过使用不同的技能卡来应对复杂的游戏场景
</div>

<strong style="font-size: 20px;">2. 音频体验</strong>

音效设计在营造沉浸感方面起到了重要作用。背景音乐会根据游戏情况动态变化：

①在游戏开始时，音乐低沉而压抑；

②在紧张时刻，音乐节奏加快，增强战斗氛围。

<strong style="font-size: 18px;">特定音效设计</strong>

①吞噬模式（红色）： 低沉缓慢的声音强调玩家沉重的动作，同时伴有微弱的咀嚼声，表现出吸收过程。

②射击模式（白色）： 清脆的射击和撞击声突出精准和攻击感。

③病毒扩散： 伴随上升的警报声，提示威胁升级。

④卡牌升级区： 进入该区域时，时间会减缓，并伴有柔和的环境音，给予玩家短暂的决策时间。

<strong style="font-size: 24px;">基础属性</strong>

<strong style="font-size: 20px;">角色</strong>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    一个小型机器人，目标是消灭所有病毒
</div>

状态

等级

子细胞数量

移动速度

毒素抗性

物理抗性

子弹伤害与速度

毒素积累： 随时间增加或减少

生命值： 基础生命值 + 子细胞总生命值（子细胞优先消耗）

饱食度： 当饱食度满时，玩家会分裂出新的子细胞，完成一次升级，并重置饱食度数值


<strong style="font-size: 20px;">1. 背景与游戏场景</strong>

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
