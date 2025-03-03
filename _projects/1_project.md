---
layout: page
title: project 1
description: ARPG 项目关卡白盒
img: assets/img/ARPG_Blockout.jpg
importance: 1
category: work
related_publications: true
---

本关卡的主要玩法是动作冒险，包含基础战斗、跑跳、探索等核心机制。整体游玩时间预计为20-25分钟，涵盖跑图、战斗、探索以及Boss战等环节。

该关卡的定位是前期连接前两个区域的辅助路线，类似于《艾尔登法环》中史东薇尔城的主干道和断崖路线的关系，提供一条与主线并行的探索路径。

故事设定在中世纪背景下，玩家在前往第二个区域的途中，由于主干道被重兵把守，无法直接通过，只能选择这条较为隐蔽的路线，寻找突破口，最终抵达目标区域。

</div>

关卡全览

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/All.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

区域1

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Area 1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

区域2

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Area 2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

区域3

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Area 3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
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
<div class="caption">
    This image can also have a caption. It's like magic.
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
