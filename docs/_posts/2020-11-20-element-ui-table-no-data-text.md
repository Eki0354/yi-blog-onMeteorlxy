---
category: quiz
tags:
  - quiz
  - 面试
date: 2020-11-20
title: 画一个可拖拽矩形
---

如题

<!-- more -->

**一个经典面试题：编写代码画一个矩形，拖拽矩形4个角中的一个，可以使矩形基于这个角进行缩放，在矩形内其他区域按住拖动可以移动该矩形的位置。**

这其实是非常基础的对于mouse相关事件的运用，但是为了~~凑字数~~更接近于真实图形绘制，还是用canvas来做。

首先当然是给出一个canvas元素并且获取到：

``` js html
  <!-- html -->
  // canvas元素
  <canvas id="canvas-eki" width="800" height="600"></canvas>

  <!-- javascript -->
  // 获取dom元素
  const canvas = document.getElementById('canvas-eki');
  // 获取canvas操作上下文，所有基于canvas的图形操作都通过其完成，当然，是可以选择'3d'模式的
  const context = canvas.getContext('2d');
```
