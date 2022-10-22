# html-css-js

## 工具

1. VS Code
2. Live Server

## 概述

1. HTML是网页内容的载体。内容就是网页制作者放在页面上想要让用户浏览的信息，可以包含文字、图片、视频等。

2. CSS样式是表现。就像网页的外衣。比如，标题字体、颜色变化，或为标题加入背景图片、边框等。所有这些用来改变内容外观的东西称之为表现。

3. JavaScript是用来实现网页上的特效效果。如：鼠标滑过弹出下拉菜单。或鼠标滑过表格的背景颜色改变。还有焦点新闻（新闻图片）的轮换。可以这么理解，有动画的，有交互的一般都是用JavaScript来实现的。

## HTML（系统骨架）

https://www.w3.org/TR/html5

Hypertext Markup Language (HTML)：超文本标记语言

1. 元素Element：HTML 元素以开始标签起始，HTML 元素以结束标签终止，元素的内容是开始标签与结束标签之间的内容，某些 HTML 元素具有空内容（empty content），空元素在开始标签中进行关闭（以开始标签的结束而结束），大多数 HTML 元素可拥有属性。元素和标签不是同一种概念。源代码中的标签用来标识元素的开始或结束，而元素是文档对象模型（DOM）中的一部分，文档对象模型会被浏览器渲染、展示为页面。https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element，https://developer.mozilla.org/zh-CN/docs/Glossary/Element。
2. 标签Tag（html）：Tags are used to delimit the start and end of elements in the markup.
3. 属性Attribute（id, title, onclick）：Attributes for an element are expressed inside the element's start tag.
4. 元数据Meta（link，script，style，title）

HTML 文档是由 HTML 元素定义的。

https://developer.mozilla.org/zh-CN/docs/Learn/Getting_started_with_the_web/HTML_basics

元素<p class="editor-note">My cat is very grumpy</p>的主要部分有：
1. 开始标签（Opening tag）：包含元素的名称（本例为 p），被大于号、小于号所包围。表示元素从这里开始或者开始起作用 —— 在本例中即段落由此开始。
2. 结束标签（Closing tag）：与开始标签相似，只是其在元素名之前包含了一个斜杠。这表示着元素的结尾 —— 在本例中即段落在此结束。初学者常常会犯忘记包含结束标签的错误，这可能会产生一些奇怪的结果。
3. 内容（Content）：元素的内容，本例中就是所输入的文本本身。
4. 元素（Element）：开始标签、结束标签与内容相结合，便是一个完整的元素。
    1. 元素也可以有属性（Attribute）：属性包含了关于元素的一些额外信息，这些信息本身不应显现在内容中。本例中，class 是属性名称，editor-note 是属性的值。class 属性可为元素提供一个标识名称，以便进一步为元素指定样式或进行其他操作时使用。

## CSS（系统静态美观）

CSS removed the style formatting from the HTML page!

层叠、优先级和继承

1. 选择器（Selector）
   1. 类型、类和 ID 选择器
   2. 标签属性选择器
   3. 伪类与伪元素
   4. 运算符
2. 盒子模型（Box Model）
   1. 块级盒子（Block box）
   2. 内联盒子（Inline box）
3. display
   1. A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can).
   2. An inline element does not start on a new line and only takes up as much width as necessary.
   3. display: none; is commonly used with JavaScript to hide and show elements without deleting and recreating them. Take a look at our last example on this page if you want to know how this can be achieved.
4. 浮动（float）
   1. The float property is used for positioning and formatting content e.g. let an image float left to the text in a container.
   2. The float property can have one of the following values:
    left - The element floats to the left of its container
    right - The element floats to the right of its container
    none - The element does not float (will be displayed just where it occurs in the text). This is default
    inherit - The element inherits the float value of its parent
5. 定位（position）
   1. static：它是position的默认值，一般不设置position属性时，元素会按照正常的文档流进行排列。
   2. relative：relative属性，我们只要搞清它是相对哪个对象来进行偏移的就ok了，答案是它原本的位置。需要注意的是，相对定位不会脱离文档流，原来的位置仍然被保留。
   3. absolute：当一个元素设置了position:absolute属性之后，而它的父级元素的属性为position:relative时，它不再是相对于文档定位，而是相对于父元素定位。最重要的是，父元素设置为position:relative并不会脱离文档流，也就是说利用给父元素设置position:relative属性，再将子元素设置为position:absolute就可以在文档流中实现需要的定位，这是一种常见的方法。
   4. fix：脱离文档流，相对于浏览器窗口定位。
   5. sticky：根据用户的滚动位置进行定位。
6. 伪类
7. Flex布局

## JavaScript（系统动态）

1. 