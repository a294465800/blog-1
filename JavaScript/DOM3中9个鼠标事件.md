---
title: DOM3中9个鼠标事件
tags:
  - DOM3
  - 鼠标事件
categories: JavaScript
date: 2017-07-27 09:51:33
---

今天看到一篇描述 `click` 事件的发生的条件, 需要同时满足 `mousedown` 和 `mouseup` 事件,
也就是鼠标按下和抬起行为在同一个元素触发才会触发 `click`.

另外找出 DOM3 中的9个鼠标事件回顾一下:

1. click

在用户单击主鼠标按钮（一般是左边的按钮）或者按下回车键时触发。这一点对确保易访问性很重要，意味着onclick事件处理程序既可以通过键盘也可以通过鼠标执行.

2. dblclick

在用户双击主鼠标按钮（一般是左边的按钮）时触发。从技术上说，这个事件并不是DOM2级事件规范中规定的，但鉴于它得到了广泛支持，所以DOM3 级事件将其纳入了标准

3. mousedown

在用户按下了任意鼠标按钮时触发。不能通过键盘触发这个事件.

4. mouseup

在用户释放鼠标按钮时触发。不能通过键盘触发这个事件.

5. mouseenter

在鼠标光标从元素外部首次移动到元素范围之内时触发。这个事件不冒泡，而且在光标移动到后代元素上不会触发。DOM2级事件并没有定义这个事件，但 DOM3级事件将它纳入了规范。IE、Firefox 9+和 Opera支持这个事件.

6. mouseleave

在位于元素上方的鼠标光标移动到元素范围之外时触发。这个事件不冒泡，而且在光标移动到后代元素上不会触发。DOM2级事件并没有定义这个事件，但
DOM3级事件将它 纳入了规范。IE、Firefox 9+和 Opera支持这个事件.

7. mousemove

当鼠标在元素内部移动时触发事件, 可以获得 client&screen 坐标.

8. mouseover

鼠标移入元素时触发事件, 会冒泡到子父代元素.

9. mouseout

鼠标移出元素时触发事件, 会冒泡到子父代元素.