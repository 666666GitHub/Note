# 1. CSS3基础

**CSS** (Cascading Style Sheets，层叠样式表），是一种用来为结构化文档（如 HTML 文档或 XML 应用）添加样式（字体、间距和颜色等）的计算机语言，**CSS** 文件扩展名为 **.css**。

通过使用 **CSS** 我们可以大大提升网页开发的工作效率！

在我们的 **CSS** 教程中，您会学到如何使用 CSS 同时控制多重网页的样式和布局。

**CSS3** 现在已被大部分现代浏览器支持

[CSS 样式优先级](https://www.runoob.com/w3cnote/css-style-priority.html)

~~~

~~~

## 1.1 选择器

[CSS 样式优先级](https://www.runoob.com/w3cnote/css-style-priority.html)

选择器{属性名：属性值；}

CSS选择器用于选择你想要的元素的样式的模式。

"CSS"列表示在CSS版本的属性定义（CSS1，CSS2，或对CSS3）。

- **ID 选择器**， 如 #id{}
  - 大多是配合JavaScript使用，很少来设置CSS样式，HTML元素以id属性来设置id选择器,CSS 中 id 选择器以 "#" 来定义。
- **类选择器**， 如 .class{}
  - class 选择器用于描述一组元素的样式，class 选择器有别于id选择器，class可以在多个元素中使用。
- 属性选择器， 如 a[href="segmentfault.com"]{}
- 伪类选择器， 如 :hover{}
- 伪元素选择器， 如 ::before{}
- **标签选择器**， 如 span{}
- **通配选择器**， 如 *{}

| 名称             | 选择器                                                       | 示例                  | 示例说明                                                   | CSS  |
| ---------------- | :----------------------------------------------------------- | :-------------------- | :--------------------------------------------------------- | :--- |
| 类选择器         | [.*class*](https://www.runoob.com/cssref/sel-class.html)     | .intro                | 选择所有class="intro"的元素                                | 1    |
| id选择器         | [#*id*](https://www.runoob.com/cssref/sel-id.html)           | #firstname            | 选择所有id="firstname"的元素                               | 1    |
| 通配符选择器     | [*](https://www.runoob.com/cssref/sel-all.html)              | *                     | 选择所有元素                                               | 2    |
| 标签选择器       | *[element](https://www.runoob.com/cssref/sel-element.html)*  | p                     | 选择所有\<p>元素                                           | 1    |
| 分组选择器       | *[element,element](https://www.runoob.com/cssref/sel-element-comma.html)* | div,p                 | 选择所有\<div>元素和\<p>元素                               | 1    |
| **CSS 的选择符** | [*element* *element*](https://www.runoob.com/cssref/sel-element-element.html) | div p                 | 选择\<div>元素内的所有\<p>元素                             | 1    |
|                  | [*element*>*element*](https://www.runoob.com/cssref/sel-element-gt.html) | div>p                 | 选择所有父级是 \<div> 元素的\<p> 元素                      | 2    |
|                  | [*element*+*element*](https://www.runoob.com/cssref/sel-element-pluss.html) | div+p                 | 选择所有紧跟在\<div> 元素之后的第一个 \<p> 元素            | 2    |
|                  | [*attribute*](https://www.runoob.com/cssref/sel-attribute.html)(属性) | [target]              | 选择所有带有target属性元素                                 | 2    |
|                  | [*attribute*=*value*](https://www.runoob.com/cssref/sel-attribute-value.html) | [target=-blank]       | 选择所有使用target="-blank"的元素                          | 2    |
|                  | [*attribute*~=*value*](https://www.runoob.com/cssref/sel-attribute-value-contains.html) | [title~=flower]       | 选择标题属性包含单词"flower"的所有元素                     | 2    |
|                  | [*attribute*\|=*language*](https://www.runoob.com/cssref/sel-attribute-value-lang.html) | [lang\|=en]           | 选择 lang 属性等于 **en**，或者以 **en-** 为开头的所有元素 | 2    |
|                  | [:link](https://www.runoob.com/cssref/sel-link.html)         | a:link                | 选择所有未访问链接                                         | 1    |
|                  | [:visited](https://www.runoob.com/cssref/sel-visited.html)   | a:visited             | 选择所有访问过的链接                                       | 1    |
|                  | [:active](https://www.runoob.com/cssref/sel-active.html)     | a:active              | 选择活动链接                                               | 1    |
|                  | [:hover](https://www.runoob.com/cssref/sel-hover.html)       | a:hover               | 选择鼠标在链接上面时                                       | 1    |
|                  | [:focus](https://www.runoob.com/cssref/sel-focus.html)       | input:focus           | 选择具有焦点的输入元素                                     | 2    |
|                  | [:first-letter](https://www.runoob.com/cssref/sel-firstletter.html) | p:first-letter        | 选择每一个\<p>元素的第一个字母                             | 1    |
|                  | [:first-line](https://www.runoob.com/cssref/sel-firstline.html) | p:first-line          | 选择每一个\<p>元素的第一行                                 | 1    |
|                  | [:first-child](https://www.runoob.com/cssref/sel-firstchild.html) | p:first-child         | 指定只有当\<p>元素是其父级的第一个子级的样式。             | 2    |
|                  | [:before](https://www.runoob.com/cssref/sel-before.html)     | p:before              | 在每个\<p>元素之前插入内容                                 | 2    |
|                  | [:after](https://www.runoob.com/cssref/sel-after.html)       | p:after               | 在每个\<p>元素之后插入内容                                 | 2    |
|                  | [:lang(*language*)](https://www.runoob.com/cssref/sel-lang.html) | p:lang(it)            | 选择一个lang属性的起始值="it"的所有\<p>元素                | 2    |
|                  | [*element1*~*element2*](https://www.runoob.com/cssref/sel-gen-sibling.html) | p~ul                  | 选择p元素之后的每一个ul元素                                | 3    |
|                  | [*attribute*^=*value*](https://www.runoob.com/cssref/sel-attr-begin.html) | a[src^="https"]       | 选择每一个src属性的值以"https"开头的元素                   | 3    |
|                  | [*attribute*$=*value*](https://www.runoob.com/cssref/sel-attr-end.html) | a[src$=".pdf"]        | 选择每一个src属性的值以".pdf"结尾的元素                    | 3    |
|                  | [*attribute**=*value*](https://www.runoob.com/cssref/sel-attr-contain.html) | a[src*="runoob"]      | 选择每一个src属性的值包含子字符串"runoob"的元素            | 3    |
|                  | [:first-of-type](https://www.runoob.com/cssref/sel-first-of-type.html) | p:first-of-type       | 选择每个p元素是其父级的第一个p元素                         | 3    |
|                  | [:last-of-type](https://www.runoob.com/cssref/sel-last-of-type.html) | p:last-of-type        | 选择每个p元素是其父级的最后一个p元素                       | 3    |
|                  | [:only-of-type](https://www.runoob.com/cssref/sel-only-of-type.html) | p:only-of-type        | 选择每个p元素是其父级的唯一p元素                           | 3    |
|                  | [:only-child](https://www.runoob.com/cssref/sel-only-child.html) | p:only-child          | 选择每个p元素是其父级的唯一子元素                          | 3    |
|                  | [:nth-child(*n*)](https://www.runoob.com/cssref/sel-nth-child.html) | p:nth-child(2)        | 选择每个p元素是其父级的第二个子元素                        | 3    |
|                  | [:nth-last-child(*n*)](https://www.runoob.com/cssref/sel-nth-last-child.html) | p:nth-last-child(2)   | 选择每个p元素的是其父级的第二个子元素，从最后一个子项计数  | 3    |
|                  | [:nth-of-type(*n*)](https://www.runoob.com/cssref/sel-nth-of-type.html) | p:nth-of-type(2)      | 选择每个p元素是其父级的第二个p元素                         | 3    |
|                  | [:nth-last-of-type(*n*)](https://www.runoob.com/cssref/sel-nth-last-of-type.html) | p:nth-last-of-type(2) | 选择每个p元素的是其父级的第二个p元素，从最后一个子项计数   | 3    |
|                  | [:last-child](https://www.runoob.com/cssref/sel-last-child.html) | p:last-child          | 选择每个p元素是其父级的最后一个子级。                      | 3    |
|                  | [:root](https://www.runoob.com/cssref/sel-root.html)         | :root                 | 选择文档的根元素                                           | 3    |
|                  | [:empty](https://www.runoob.com/cssref/sel-empty.html)       | p:empty               | 选择每个没有任何子级的p元素（包括文本节点）                | 3    |
|                  | [:target](https://www.runoob.com/cssref/sel-target.html)     | #news:target          | 选择当前活动的#news元素（包含该锚名称的点击的URL）         | 3    |
|                  | [:enabled](https://www.runoob.com/cssref/sel-enabled.html)   | input:enabled         | 选择每一个已启用的输入元素                                 | 3    |
|                  | [:disabled](https://www.runoob.com/cssref/sel-disabled.html) | input:disabled        | 选择每一个禁用的输入元素                                   | 3    |
|                  | [:checked](https://www.runoob.com/cssref/sel-checked.html)   | input:checked         | 选择每个选中的输入元素                                     | 3    |
|                  | [:not(*selector*)](https://www.runoob.com/cssref/sel-not.html) | :not(p)               | 选择每个并非p元素的元素                                    | 3    |
|                  | [::selection](https://www.runoob.com/cssref/sel-selection.html) | ::selection           | 匹配元素中被用户选中或处于高亮状态的部分                   | 3    |
|                  | [:out-of-range](https://www.runoob.com/cssref/sel-out-of-range.html) | :out-of-range         | 匹配值在指定区间之外的input元素                            | 3    |
|                  | [:in-range](https://www.runoob.com/cssref/sel-in-range.html) | :in-range             | 匹配值在指定区间之内的input元素                            | 3    |
|                  | [:read-write](https://www.runoob.com/cssref/sel-read-write.html) | :read-write           | 用于匹配可读及可写的元素                                   | 3    |
|                  | [:read-only](https://www.runoob.com/cssref/sel-read-only.html) | :read-only            | 用于匹配设置 "readonly"（只读） 属性的元素                 | 3    |
|                  | [:optional](https://www.runoob.com/cssref/sel-optional.html) | :optional             | 用于匹配可选的输入元素                                     | 3    |
|                  | [:required](https://www.runoob.com/cssref/sel-required.html) | :required             | 用于匹配设置了 "required" 属性的元素                       | 3    |
|                  | [:valid](https://www.runoob.com/cssref/sel-valid.html)       | :valid                | 用于匹配输入值为合法的元素                                 | 3    |
|                  | [:invalid](https://www.runoob.com/cssref/sel-invalid.html)   | :invalid              | 用于匹配输入值为非法的元素                                 | 3    |

### 1.1.1  CSS 7 种基础的选择器

---

- **ID 选择器**， 如 #id{}
  - 大多是配合JavaScript使用，很少来设置CSS样式，HTML元素以id属性来设置id选择器,CSS 中 id 选择器以 "#" 来定义。
- **类选择器**， 如 .class{}
  - class 选择器用于描述一组元素的样式，class 选择器有别于id选择器，class可以在多个元素中使用。
- 属性选择器， 如 a[href="segmentfault.com"]{}
- 伪类选择器， 如 :hover{}
- 伪元素选择器， 如 ::before{}
- **标签选择器**， 如 span{}
- **通配选择器**， 如 *{}



**CSS 优先规则3：**优先级关系：!important > 内联样式 > ID 选择器 > 类选择器 = 属性选择器 = 伪类选择器 > 标签选择器 = 伪元素选择器

**(标签范围越大，优先级越低)**

所有 **CSS 的选择符**由上述 7 种基础的选择器或者组合而成，组合的方式有 3 种：

- 后代选择符： .father .child{}

- 子选择符： .father > .child{}

- 相邻选择符: .bro1 + .bro2{}

  - ~~~css
    div,p,span{
    
    }
    ~~~

    
    



CSS引入方式

+ [内部样式表](内部样式表)：学习使用

  + CSS代码写在style标签里面
  + 相同属性会覆盖：后面的属性覆盖前面的属性
  + 不同属性会叠加：不同的属性会叠加都生效

+ [外部样式表](https://www.runoob.com/css/css-howto.html)：开发使用

  + CSS代码写在单独的CSS文件中（.css）
  + 在使用HTML中使用[\<link>](https://www.runoob.com/tags/tag-link.html)标签引入

+ [内联样式](https://www.runoob.com/css/css-howto.html)：配合JavaScript使用

  + CSS写在标签的style属性值里

+ [多重样式](https://www.runoob.com/css/css-howto.html)：如果某些属性在不同的样式表中被同样的选择器定义，那么属性值将从更具体的样式表中被继承过来。 

  + **多重样式优先级：**样式表允许以多种方式规定样式信息。样式可以规定在单个的 HTML 元素中，在 HTML 页的头元素中，或在一个外部的 CSS 文件中。甚至可以在同一个 HTML 文档内部引用多个外部样式表。

    一般情况下，优先级如下：

    **（内联样式）Inline style > （内部样式）Internal style sheet >（外部样式）External style sheet > 浏览器默认样式**

## 1.2 CSS 盒子模型

[CSS盒子模型](https://www.runoob.com/css/css-boxmodel.html)

![CSS box-model](CSS3笔记.assets/box-model.gif)

## 1.3 文本

[CSS文本](https://www.runoob.com/css/css-text.html)

**所有CSS文本属性。**

| 属性                                                         | 描述                     |
| :----------------------------------------------------------- | :----------------------- |
| [color](https://www.runoob.com/cssref/pr-text-color.html)    | 设置文本颜色             |
| [direction](https://www.runoob.com/cssref/pr-text-direction.html) | 设置文本方向。           |
| [letter-spacing](https://www.runoob.com/cssref/pr-text-letter-spacing.html) | 设置字符间距             |
| [line-height](https://www.runoob.com/cssref/pr-dim-line-height.html) | 设置行高                 |
| [text-align](https://www.runoob.com/cssref/pr-text-text-align.html) | 对齐元素中的文本         |
| [text-decoration](https://www.runoob.com/cssref/pr-text-text-decoration.html) | 向文本添加修饰           |
| [text-indent](https://www.runoob.com/cssref/pr-text-text-indent.html) | 缩进元素中文本的首行     |
| [text-shadow](https://www.runoob.com/cssref/css3-pr-text-shadow.html) | 设置文本阴影             |
| [text-transform](https://www.runoob.com/cssref/pr-text-text-transform.html) | 控制元素中的字母         |
| [unicode-bidi](https://www.runoob.com/cssref/pr-text-unicode-bidi.html) | 设置或返回文本是否被重写 |
| [vertical-align](https://www.runoob.com/cssref/pr-pos-vertical-align.html) | 设置元素的垂直对齐       |
| [white-space](https://www.runoob.com/cssref/pr-text-white-space.html) | 设置元素中空白的处理方式 |
| [word-spacing](https://www.runoob.com/cssref/pr-text-word-spacing.html) | 设置字间距               |



## 1.4 字体

[CSS字体](https://www.runoob.com/css/css-font.html)

**所有CSS字体属性**

| [font](https://www.runoob.com/cssref/pr-font-font.html)      | 在一个声明中设置所有的字体属性       |
| ------------------------------------------------------------ | ------------------------------------ |
| [font-family](https://www.runoob.com/cssref/pr-font-font-family.html) | 指定文本的字体系列                   |
| [font-size](https://www.runoob.com/cssref/pr-font-font-size.html) | 指定文本的字体大小                   |
| [font-style](https://www.runoob.com/cssref/pr-font-font-style.html) | 指定文本的字体样式                   |
| [font-variant](https://www.runoob.com/cssref/pr-font-font-variant.html) | 以小型大写字体或者正常字体显示文本。 |
| [font-weight](https://www.runoob.com/cssref/pr-font-weight.html) | 指定字体的粗细。                     |

## 1.5 背景

[CSS背景](https://www.runoob.com/css/css-background.html)

**写法：**

+ 拆分写法
+ 复合写法

## 1.6 显示模式

[显示模式](https://www.runoob.com/css/css-display-visibility.html)

+ 块级元素
  + 独占一行
  + 默认是父级的100%
  + 添加宽高属性生效
+ 行内元素
  + 行内共存几个
  + 默认尺寸由内容撑开
  + 添加宽高属性不生效
+ 行内块元素
  + 行内共存几个
  + 默认尺寸由内容撑开

## CSS 背景属性

| Property                                                     | 描述                                         |
| :----------------------------------------------------------- | :------------------------------------------- |
| [background](https://www.runoob.com/cssref/css3-pr-background.html) | 简写属性，作用是将背景属性设置在一个声明中。 |
| [background-attachment](https://www.runoob.com/cssref/pr-background-attachment.html) | 背景图像是否固定或者随着页面的其余部分滚动。 |
| [background-color](https://www.runoob.com/cssref/pr-background-color.html) | 设置元素的背景颜色。                         |
| [background-image](https://www.runoob.com/cssref/pr-background-image.html) | 把图像设置为背景。                           |
| [background-position](https://www.runoob.com/cssref/pr-background-position.html) | 设置背景图像的起始位置。                     |
| [background-repeat](https://www.runoob.com/cssref/pr-background-repeat.html) | 设置背景图像是否及如何重复。                 |

# HTML标签（按功能分类）

### 1. 基础元素

| 标签                                                        | 描述               |
| :---------------------------------------------------------- | :----------------- |
| **基础**                                                    |                    |
| [\<!DOCTYPE>](https://www.runoob.com/tags/tag-doctype.html) | 定义文档类型。     |
| [\<html>](https://www.runoob.com/tags/tag-html.html)        | 定义一个 HTML 文档 |
| [\<title>](https://www.runoob.com/tags/tag-title.html)      | 为文档定义一个标题 |
| [\<body>](https://www.runoob.com/tags/tag-body.html)        | 定义文档的主体     |
| [ \<h> ](https://www.runoob.com/tags/tag-hn.html)           | 定义 HTML 标题     |
| [\<p>](https://www.runoob.com/tags/tag-p.html)              | 定义一个段落       |
| [\<br>](https://www.runoob.com/tags/tag-br.html)            | 定义简单的折行。   |
| [\<hr>](https://www.runoob.com/tags/tag-hr.html)            | 定义水平线。       |
| [\<!-- -->](https://www.runoob.com/tags/tag-comment.html)   | 定义一个注释       |

### 2. 格式标签

| 标签                                                         | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| **格式**                                                     |                                                              |
| [\<abbr>](https://www.runoob.com/tags/tag-abbr.html)         | 定义一个缩写。                                               |
| [\<address>](https://www.runoob.com/tags/tag-address.html)   | 定义文档作者或拥有者的联系信息。                             |
| [\<b>](https://www.runoob.com/tags/tag-b.html)               | 定义粗体文本。                                               |
| [\<bdi>](https://www.runoob.com/tags/tag-bdi.html)**New**    | 允许您设置一段文本，使其脱离其父元素的文本方向设置。         |
| [\<bdo>](https://www.runoob.com/tags/tag-bdo.html)           | 定义文本的方向。                                             |
| [\<blockquote>](https://www.runoob.com/tags/tag-blockquote.html) | 定义块引用。                                                 |
| [\<cite>](https://www.runoob.com/tags/tag-cite.html)         | 定义引用(citation)。                                         |
| [\<code>](https://www.runoob.com/tags/tag-code.html)         | 定义计算机代码文本。                                         |
| [\<del>](https://www.runoob.com/tags/tag-del.html)           | 定义被删除文本。                                             |
| [\<dfn>](https://www.runoob.com/tags/tag-dfn.html)           | 定义定义项目。                                               |
| [\<em>](https://www.runoob.com/tags/tag-em.html)             | 定义强调文本。                                               |
| [\<i>](https://www.runoob.com/tags/tag-i.html)               | 定义斜体文本。                                               |
| [\<ins>](https://www.runoob.com/tags/tag-ins.html)           | 定义被插入文本。                                             |
| [\<kbd>](https://www.runoob.com/tags/tag-kbd.html)           | 定义键盘文本。                                               |
| [\<mark>](https://www.runoob.com/tags/tag-mark.html)**New**  | 定义带有记号的文本。                                         |
| [\<meter>](https://www.runoob.com/tags/tag-meter.html)**New** | 定义度量衡。仅用于已知最大和最小值的度量。                   |
| [\<pre>](https://www.runoob.com/tags/tag-pre.html)           | 定义预格式文本                                               |
| [\<progress>](https://www.runoob.com/tags/tag-progress.html)**New** | 定义运行中的任务进度（进程）。                               |
| [\<q>](https://www.runoob.com/tags/tag-q.html)               | 定义短的引用。                                               |
| [\<rp>](https://www.runoob.com/tags/tag-rp.html)**New**      | 定义不支持 ruby 元素的浏览器所显示的内容。                   |
| [\<rt>](https://www.runoob.com/tags/tag-rt.html)**New**      | 定义字符（中文注音或字符）的解释或发音。                     |
| [\<ruby>](https://www.runoob.com/tags/tag-ruby.html)**New**  | 定义 ruby 注释（中文注音或字符）。                           |
| [\<s>](https://www.runoob.com/tags/tag-s.html)               | 定义加删除线的文本。                                         |
| [\<samp>](https://www.runoob.com/tags/tag-samp.html)         | 定义计算机代码样本。                                         |
| [\<small>](https://www.runoob.com/tags/tag-small.html)       | 定义小号文本。                                               |
| [\<strong>](https://www.runoob.com/tags/tag-strong.html)     | 定义语气更为强烈的强调文本。                                 |
| [\<sub>](https://www.runoob.com/tags/tag-sub.html)           | 定义下标文本。                                               |
| [\<sup>](https://www.runoob.com/tags/tag-sup.html)           | 定义上标文本。                                               |
| [\<time>](https://www.runoob.com/tags/tag-time.html)**New**  | 定义一个日期/时间                                            |
| [\<u>](https://www.runoob.com/tags/tag-u.html)               | 定义下划线文本。                                             |
| [\<var>](https://www.runoob.com/tags/tag-var.html)           | 定义文本的变量部分。                                         |
| [\<wbr>](https://www.runoob.com/tags/tag-wbr.html)**New**    | 规定在文本中的何处适合添加换行符。                           |
| [\<center>](https://www.runoob.com/tags/tag-center.html)     | HTML5不再支持。 HTML 4.01 已废弃。定义居中文本。             |
| [\<big>](https://www.runoob.com/tags/tag-big.html)           | HTML5不再支持。 定义大号文本。                               |
| [\<acronym>](https://www.runoob.com/tags/tag-acronym.html)   | HTML5不再支持。 定义只取首字母的缩写。                       |
| [\<font>](https://www.runoob.com/tags/tag-font.html)         | HTML5不再支持。 HTML 4.01 已废弃。 定义文本的字体、尺寸和颜色 |
| [\<tt>](https://www.runoob.com/tags/tag-tt.html)             | HTML5不再支持。 定义打字机文本。                             |
| [\<strike>](https://www.runoob.com/tags/tag-strike.html)     | HTML5不再支持。 HTML 4.01 已废弃。 定义加删除线的文本。      |

### 3. 表单

| 标签                                                         | 描述                               |
| :----------------------------------------------------------- | :--------------------------------- |
| **表单**                                                     |                                    |
| [\<form>](https://www.runoob.com/tags/tag-form.html)         | 定义一个 HTML 表单，用于用户输入。 |
| [\<input>](https://www.runoob.com/tags/tag-input.html)       | 定义一个输入控件                   |
| [\<textarea>](https://www.runoob.com/tags/tag-textarea.html) | 定义多行的文本输入控件。           |
| [\<button>](https://www.runoob.com/tags/tag-button.html)     | 定义按钮。                         |
| [\<select>](https://www.runoob.com/tags/tag-select.html)     | 定义选择列表（下拉列表）。         |
| [\<optgroup>](https://www.runoob.com/tags/tag-optgroup.html) | 定义选择列表中相关选项的组合。     |
| [\<option>](https://www.runoob.com/tags/tag-option.html)     | 定义选择列表中的选项。             |
| [\<label>](https://www.runoob.com/tags/tag-label.html)       | 定义 input 元素的标注。            |
| [\<fieldset>](https://www.runoob.com/tags/tag-fieldset.html) | 定义围绕表单中元素的边框。         |
| [\<legend>](https://www.runoob.com/tags/tag-legend.html)     | 定义 fieldset 元素的标题。         |
| [\<detail>](https://www.runoob.com/tags/tag-datalist.html)**New** | 规定了 input 元素可能的选项列表。  |
| [\<keygen>](https://www.runoob.com/tags/tag-keygen.html)**New** | 规定用于表单的密钥对生成器字段。   |
| [\<output>](https://www.runoob.com/tags/tag-output.html)**New** | 定义一个计算的结果                 |

### 4. 框架

| 标签                                                         | 描述                                                 |
| :----------------------------------------------------------- | :--------------------------------------------------- |
| **框架**                                                     |                                                      |
| [\<iframe>](https://www.runoob.com/tags/tag-iframe.html)     | 定义内联框架。                                       |
| [\<frame>](https://www.runoob.com/tags/tag-frame.html)       | HTML5不再支持。 定义框架集的窗口或框架。             |
| [\<frameset>](https://www.runoob.com/tags/tag-frameset.html) | HTML5不再支持。定义框架集。                          |
| [\<noframes>](https://www.runoob.com/tags/tag-noframes.html) | HTML5不再支持。 定义针对不支持框架的用户的替代内容。 |

### 5. 图像

| 标签                                                         | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| **图像**                                                     |                                                              |
| [\<img>](https://www.runoob.com/tags/tag-img.html)           | 定义图像。                                                   |
| [\<map>](https://www.runoob.com/tags/tag-map.html)           | 定义图像映射。                                               |
| [\<erea>](https://www.runoob.com/tags/tag-area.html)         | 定义图像地图内部的区域。                                     |
| [\<canvas>](https://www.runoob.com/tags/tag-canvas.html)**New** | 通过脚本（通常是 JavaScript）来绘制图形（比如图表和其他图像）。 |
| [\<figcaption>](https://www.runoob.com/tags/tag-figcaption.html)**New** | 定义一个 caption for a <figure> element                      |
| [\<figure>](https://www.runoob.com/tags/tag-figure.html)**New** | figure 标签用于对元素进行组合。                              |

### 6. Audio/Video

| 标签                                                         | 描述                                                |
| :----------------------------------------------------------- | :-------------------------------------------------- |
| **Audio/Video**                                              |                                                     |
| [\<audio>](https://www.runoob.com/tags/tag-audio.html)**New** | 定义声音，比如音乐或其他音频流。                    |
| [\<source>](https://www.runoob.com/tags/tag-source.html)**New** | 定义media元素 (<video> 和 <audio>)的媒体资源。media |
| [\<track>](https://www.runoob.com/tags/tag-track.html)**New** | 为媒体(<video> 和 <audio>)元素定义外部文本轨道。    |
| [\<video>](https://www.runoob.com/tags/tag-video.html)**New** | 定义一个音频或者视频                                |

### 7. 链接

| 标签                                                      | 描述                       |
| :-------------------------------------------------------- | :------------------------- |
| **链接**                                                  |                            |
| [\<a>](https://www.runoob.com/tags/tag-a.html)            | 定义一个链接               |
| [\<link>](https://www.runoob.com/tags/tag-link.html)      | 定义文档与外部资源的关系。 |
| [\<main>](https://www.runoob.com/tags/tag-main.html)      | 定义文档的主体部分。       |
| [\<nav>](https://www.runoob.com/tags/tag-nav.html)**New** | 定义导航链接               |

### 8. 列表

| 标签                                                         | 描述                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------- |
| **列表**                                                     |                                                        |
| [\<ul>](https://www.runoob.com/tags/tag-ul.html)             | 定义一个无序列表                                       |
| [\<ol>](https://www.runoob.com/tags/tag-ol.html)             | 定义一个有序列表                                       |
| [\<li>](https://www.runoob.com/tags/tag-li.html)             | 定义一个列表项                                         |
| [\<dl>](https://www.runoob.com/tags/tag-dl.html)             | 定义一个定义列表                                       |
| [\<dt>](https://www.runoob.com/tags/tag-dt.html)             | 定义一个定义定义列表中的项目。                         |
| [\<dd>](https://www.runoob.com/tags/tag-dd.html)             | 定义定义列表中项目的描述。                             |
| [\<menu>](https://www.runoob.com/tags/tag-menu.html)         | 定义菜单列表。                                         |
| [\<command>](https://www.runoob.com/tags/tag-command.html)**New** | 定义用户可能调用的命令（比如单选按钮、复选框或按钮）。 |
| [\<dir>](https://www.runoob.com/tags/tag-dir.html)           | HTML5不再支持。 HTML 4.01 已废弃。 定义目录列表。      |

### 9. 表格

| 标签                                                         | 描述                             |
| :----------------------------------------------------------- | :------------------------------- |
| **表格**                                                     |                                  |
| [\<table>](https://www.runoob.com/tags/tag-table.html)       | 定义一个表格                     |
| [\<caption>](https://www.runoob.com/tags/tag-caption.html)   | 定义表格标题。                   |
| [\<th>](https://www.runoob.com/tags/tag-th.html)             | 定义表格中的表头单元格。         |
| [\<tr>]()                                                    | 定义表格中的行。                 |
| [\<td>](https://www.runoob.com/tags/tag-td.html)             | 定义表格中的单元。               |
| [\<thead>]()                                                 | 定义表格中的表头内容。           |
| [\<tbody>](https://www.runoob.com/tags/tag-tbody.html)       | 定义表格中的主体内容。           |
| [\<tfoot>](https://www.runoob.com/tags/tag-tfoot.html)       | 定义表格中的表注内容（脚注）。   |
| [\<col>](https://www.runoob.com/tags/tag-col.html)           | 定义表格中一个或多个列的属性值。 |
| [\<colgroup>](https://www.runoob.com/tags/tag-colgroup.html) | 定义表格中供格式化的列组。       |

### 10. 样式/节

| 标签                                                         | 描述                                                    |
| :----------------------------------------------------------- | :------------------------------------------------------ |
| **样式/节**                                                  |                                                         |
| [\<stytle>](https://www.runoob.com/tags/tag-style.html)      | 定义文档的样式信息。                                    |
| [\<div>](https://www.runoob.com/tags/tag-div.html)           | 定义文档中的节。                                        |
| [\<span>](https://www.runoob.com/tags/tag-span.html)         | 定义文档中的节。                                        |
| [\<header>](https://www.runoob.com/tags/tag-header.html)**New** | 定义一个文档头部部分                                    |
| [\<footer>](https://www.runoob.com/tags/tag-footer.html)**New** | 定义一个文档底部                                        |
| [\<section>](https://www.runoob.com/tags/tag-section.html)**New** | 定义了文档的某个区域                                    |
| [\<article>](https://www.runoob.com/tags/tag-article.html)**New** | 定义一个文章内容                                        |
| [\<aside>](https://www.runoob.com/tags/tag-aside.html)**New** | 定义其所处内容之外的内容。                              |
| [\<details>](https://www.runoob.com/tags/tag-details.html)**New** | 定义了用户可见的或者隐藏的需求的补充细节。              |
| [\<dialog>](https://www.runoob.com/tags/tag-dialog.html)**New** | 定义一个对话框或者窗口                                  |
| [\<summary>](https://www.runoob.com/tags/tag-summary.html)**New** | 定义一个可见的标题。 当用户点击标题时会显示出详细信息。 |

### 11. 元信息

| 标签                                                         | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| **元信息**                                                   |                                                              |
| [\<head>](https://www.runoob.com/tags/tag-head.html)         | 定义关于文档的信息                                           |
| [\<meta>](https://www.runoob.com/tags/tag-meta.html)         | 定义关于 HTML 文档的元信息。                                 |
| [\<base>](https://www.runoob.com/tags/tag-base.html)         | 定义页面中所有链接的默认地址或默认目标。                     |
| [\<basefont>](https://www.runoob.com/tags/tag-basefont.html) | HTML5不再支持。 HTML 4.01 已废弃。 定义页面中文本的默认字体、颜色或尺寸。 |

### 12. 程序

| 标签                                                         | 描述                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------- |
| **程序**                                                     |                                                        |
| [\<script>](https://www.runoob.com/tags/tag-script.html)     | 定义客户端脚本。                                       |
| [\<noscript>](https://www.runoob.com/tags/tag-noscript.html) | 定义针对不支持客户端脚本的用户的替代内容。             |
| [\<embed>](https://www.runoob.com/tags/tag-embed.html)**New** | 定义了一个容器，用来嵌入外部应用或者互动程序（插件）。 |
| [\<object>](https://www.runoob.com/tags/tag-object.html)     | 定义嵌入的对象。                                       |
| [\<param>](https://www.runoob.com/tags/tag-param.html)       | 定义对象的参数。                                       |
| [\<applet>](https://www.runoob.com/tags/tag-applet.html)     | HTML5不再支持。 HTML 4.01 已废弃。 定义嵌入的 applet。 |

# CSS 属性（按功能分类）

## 1. background(背景)属性 

**背景属性**

| Property                                                     | 描述                                         |
| :----------------------------------------------------------- | :------------------------------------------- |
| [background](https://www.runoob.com/cssref/css3-pr-background.html) | 简写属性，作用是将背景属性设置在一个声明中。 |
| [background-attachment](https://www.runoob.com/cssref/pr-background-attachment.html) | 背景图像是否固定或者随着页面的其余部分滚动。 |
| [background-color](https://www.runoob.com/cssref/pr-background-color.html) | 设置元素的背景颜色。                         |
| [background-image](https://www.runoob.com/cssref/pr-background-image.html) | 把图像设置为背景。                           |
| [background-position](https://www.runoob.com/cssref/pr-background-position.html) | 设置背景图像的起始位置。                     |
| [background-repeat](https://www.runoob.com/cssref/pr-background-repeat.html) | 设置背景图像是否及如何重复。                 |

| Property                                                     | 描述                                              | 属性值                                                       |
| :----------------------------------------------------------- | :------------------------------------------------ | ------------------------------------------------------------ |
| [background](https://www.runoob.com/cssref/css3-pr-background.html) | 简写属性，作用是将背景属性<br/>设置在一个声明中。 | background-color <br>background-image <br/>background-repeat <br/>background-attachment <br/>background-position <br/> |

#### 1. background属性

| 值                                                           | 说明                                             | CSS  |
| :----------------------------------------------------------- | :----------------------------------------------- | :--- |
| *[background-color](https://www.runoob.com/cssref/pr-background-color.html)* | 指定要使用的背景颜色                             | 1    |
| *[background-position](https://www.runoob.com/cssref/pr-background-position.html)* | 指定背景图像的位置                               | 1    |
| *[background-attachment](https://www.runoob.com/cssref/pr-background-attachment.html)* | 设置背景图像是否固定或者随着页面的其余部分滚动。 | 1    |
| *[background-image](https://www.runoob.com/cssref/pr-background-image.html)* | 指定要使用的一个或多个背景图像                   | 1    |
| *[background-repeat](https://www.runoob.com/cssref/pr-background-repeat.html)* | 指定如何重复背景图像                             | 1    |
| *[background-origin](https://www.runoob.com/cssref/css3-pr-background-origin.html)* | 指定背景图像的定位区域                           | 3    |
| *[background-clip](https://www.runoob.com/cssref/css3-pr-background-clip.html)* | 指定背景图像的绘画区域                           | 3    |
| *[background-size](https://www.runoob.com/cssref/css3-pr-background-size.html)* | 指定背景图片的大小                               | 3    |

#### 2. background-attachment属性

| 值      | 描述                                                         |
| :------ | :----------------------------------------------------------- |
| scroll  | 背景图片随着页面的滚动而滚动，这是默认的。                   |
| fixed   | 背景图片不会随着页面的滚动而滚动。                           |
| local   | 背景图片会随着元素内容的滚动而滚动。                         |
| initial | 设置该属性的默认值。 [阅读关于 *initial* 内容](https://www.runoob.com/cssref/css-initial.html) |
| inherit | 指定 background-attachment 的设置应该从父元素继承。 [阅读关于 *inherit* 内容](https://www.runoob.com/cssref/css-inherit.html) |

#### 3.background-color属性

| 值          | 描述                                                         |
| :---------- | :----------------------------------------------------------- |
| *color*     | 指定背景颜色。在[CSS颜色值](https://www.runoob.com/css/css-colors-legal.html)近可能的寻找一个颜色值的完整列表。 |
| transparent | 指定背景颜色应该是透明的。这是默认                           |
| inherit     | 指定背景颜色，应该从父元素继承                               |

#### 4.background-image属性

| 值                                                           | 说明                                      |
| :----------------------------------------------------------- | :---------------------------------------- |
| url(*'URL'*)                                                 | 图像的URL                                 |
| none                                                         | 无图像背景会显示。这是默认                |
| [linear-gradient()](https://www.runoob.com/cssref/func-linear-gradient.html) | 创建一个线性渐变的 "图像"(从上到下)       |
| [radial-gradient()](https://www.runoob.com/cssref/func-radial-gradient.html) | 用径向渐变创建 "图像"。 (center to edges) |
| [repeating-linear-gradient()](https://www.runoob.com/cssref/func-repeating-linear-gradient.html) | 创建重复的线性渐变 "图像"。               |
| [repeating-radial-gradient()](https://www.runoob.com/cssref/func-repeating-radial-gradient.html) | 创建重复的径向渐变 "图像"                 |
| inherit                                                      | 指定背景图像应该从父元素继承              |

## 2. text（文本）属性

| 属性                                                         | 描述                     |
| :----------------------------------------------------------- | :----------------------- |
| [color](https://www.runoob.com/cssref/pr-text-color.html)    | 设置文本颜色             |
| [direction](https://www.runoob.com/cssref/pr-text-direction.html) | 设置文本方向。           |
| [letter-spacing](https://www.runoob.com/cssref/pr-text-letter-spacing.html) | 设置字符间距             |
| [line-height](https://www.runoob.com/cssref/pr-dim-line-height.html) | 设置行高                 |
| [text-align](https://www.runoob.com/cssref/pr-text-text-align.html) | 对齐元素中的文本         |
| [text-decoration](https://www.runoob.com/cssref/pr-text-text-decoration.html) | 向文本添加修饰           |
| [text-indent](https://www.runoob.com/cssref/pr-text-text-indent.html) | 缩进元素中文本的首行     |
| [text-shadow](https://www.runoob.com/cssref/css3-pr-text-shadow.html) | 设置文本阴影             |
| [text-transform](https://www.runoob.com/cssref/pr-text-text-transform.html) | 控制元素中的字母         |
| [unicode-bidi](https://www.runoob.com/cssref/pr-text-unicode-bidi.html) | 设置或返回文本是否被重写 |
| [vertical-align](https://www.runoob.com/cssref/pr-pos-vertical-align.html) | 设置元素的垂直对齐       |
| [white-space](https://www.runoob.com/cssref/pr-text-white-space.html) | 设置元素中空白的处理方式 |
| [word-spacing](https://www.runoob.com/cssref/pr-text-word-spacing.html) | 设置字间距               |

## 3. font（字体）属性

| Property                                                     | 描述                                 |
| :----------------------------------------------------------- | :----------------------------------- |
| [font](https://www.runoob.com/cssref/pr-font-font.html)      | 在一个声明中设置所有的字体属性       |
| [font-family](https://www.runoob.com/cssref/pr-font-font-family.html) | 指定文本的字体系列                   |
| [font-size](https://www.runoob.com/cssref/pr-font-font-size.html) | 指定文本的字体大小                   |
| [font-style](https://www.runoob.com/cssref/pr-font-font-style.html) | 指定文本的字体样式                   |
| [font-variant](https://www.runoob.com/cssref/pr-font-font-variant.html) | 以小型大写字体或者正常字体显示文本。 |
| [font-weight](https://www.runoob.com/cssref/pr-font-weight.html) | 指定字体的粗细。                     |

## 4. list（列表）属性

| 属性                                                         | 描述                                               |
| :----------------------------------------------------------- | :------------------------------------------------- |
| [list-style](https://www.runoob.com/cssref/pr-list-style.html) | 简写属性。用于把所有用于列表的属性设置于一个声明中 |
| [list-style-image](https://www.runoob.com/cssref/pr-list-style-image.html) | 将图像设置为列表项标志。                           |
| [list-style-position](https://www.runoob.com/cssref/pr-list-style-position.html) | 设置列表中列表项标志的位置。                       |
| [list-style-type](https://www.runoob.com/cssref/pr-list-style-type.html) | 设置列表项标志的类型。                             |

## 5. border（边框）属性

| 属性                                                         | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [border](https://www.runoob.com/cssref/pr-border.html)       | 简写属性，用于把针对四个边的属性设置在一个声明。             |
| [border-style](https://www.runoob.com/cssref/pr-border-style.html) | 用于设置元素所有边框的样式，或者单独地为各边设置边框样式。   |
| [border-width](https://www.runoob.com/cssref/pr-border-width.html) | 简写属性，用于为元素的所有边框设置宽度，或者单独地为各边边框设置宽度。 |
| [border-color](https://www.runoob.com/cssref/pr-border-color.html) | 简写属性，设置元素的所有边框中可见部分的颜色，或为 4 个边分别设置颜色。 |
| [border-bottom](https://www.runoob.com/cssref/pr-border-bottom.html) | 简写属性，用于把下边框的所有属性设置到一个声明中。           |
| [border-bottom-color](https://www.runoob.com/cssref/pr-border-bottom-color.html) | 设置元素的下边框的颜色。                                     |
| [border-bottom-style](https://www.runoob.com/cssref/pr-border-bottom-style.html) | 设置元素的下边框的样式。                                     |
| [border-bottom-width](https://www.runoob.com/cssref/pr-border-bottom-width.html) | 设置元素的下边框的宽度。                                     |
| [border-left](https://www.runoob.com/cssref/pr-border-left.html) | 简写属性，用于把左边框的所有属性设置到一个声明中。           |
| [border-left-color](https://www.runoob.com/cssref/pr-border-left-color.html) | 设置元素的左边框的颜色。                                     |
| [border-left-style](https://www.runoob.com/cssref/pr-border-left-style.html) | 设置元素的左边框的样式。                                     |
| [border-left-width](https://www.runoob.com/cssref/pr-border-left-width.html) | 设置元素的左边框的宽度。                                     |
| [border-right](https://www.runoob.com/cssref/pr-border-right.html) | 简写属性，用于把右边框的所有属性设置到一个声明中。           |
| [border-right-color](https://www.runoob.com/cssref/pr-border-right-color.html) | 设置元素的右边框的颜色。                                     |
| [border-right-style](https://www.runoob.com/cssref/pr-border-right-style.html) | 设置元素的右边框的样式。                                     |
| [border-right-width](https://www.runoob.com/cssref/pr-border-right-width.html) | 设置元素的右边框的宽度。                                     |
| [border-top](https://www.runoob.com/cssref/pr-border-top.html) | 简写属性，用于把上边框的所有属性设置到一个声明中。           |
| [border-top-color](https://www.runoob.com/cssref/pr-border-top-color.html) | 设置元素的上边框的颜色。                                     |
| [border-top-style](https://www.runoob.com/cssref/pr-border-top-style.html) | 设置元素的上边框的样式。                                     |
| [border-top-width](https://www.runoob.com/cssref/pr-border-top-width.html) | 设置元素的上边框的宽度。                                     |
| [border-radius](https://www.runoob.com/cssref/css3-pr-border-radius.html) | 设置圆角的边框。                                             |

## 6.  outline(轮廓)属性

"CSS" 列中的数字表示哪个CSS版本定义了该属性(CSS1 或者CSS2)。

| 属性                                                         | 说明                           | 值                                                           | CSS  |
| :----------------------------------------------------------- | :----------------------------- | :----------------------------------------------------------- | :--- |
| [outline](https://www.runoob.com/cssref/pr-outline.html)     | 在一个声明中设置所有的轮廓属性 | *outline-color<br> outline-style<br/> outline-width <br/>*inherit | 2    |
| [outline-color](https://www.runoob.com/cssref/pr-outline-color.html) | 设置轮廓的颜色                 | *color-name<br/> hex-number <br/>rgb-number <br/>*invert <br/>inherit | 2    |
| [outline-style](https://www.runoob.com/cssref/pr-outline-style.html) | 设置轮廓的样式                 | none <br/>dotted <br/>dashed <br/>solid <br/>double <br/>groove <br/>ridge <br/>inset <br/>outset<br/> inherit | 2    |
| [outline-width](https://www.runoob.com/cssref/pr-outline-width.html) | 设置轮廓的宽度                 | thin<br/> medium <br/>thick<br/> *length <br/>*inherit       | 2    |

## 7. margin(外边距)边距属性

| 属性                                                         | 描述                                       |
| :----------------------------------------------------------- | :----------------------------------------- |
| [margin](https://www.runoob.com/cssref/pr-margin.html)       | 简写属性。在一个声明中设置所有外边距属性。 |
| [margin-bottom](https://www.runoob.com/cssref/pr-margin-bottom.html) | 设置元素的下外边距。                       |
| [margin-left](https://www.runoob.com/cssref/pr-margin-left.html) | 设置元素的左外边距。                       |
| [margin-right](https://www.runoob.com/cssref/pr-margin-right.html) | 设置元素的右外边距。                       |
| [margin-top](https://www.runoob.com/cssref/pr-margin-top.html) | 设置元素的上外边距。                       |

## 8. padding（填充）属性

| 属性                                                         | 说明                                       |
| :----------------------------------------------------------- | :----------------------------------------- |
| [padding](https://www.runoob.com/cssref/pr-padding.html)     | 使用简写属性设置在一个声明中的所有填充属性 |
| [padding-bottom](https://www.runoob.com/cssref/pr-padding-bottom.html) | 设置元素的底部填充                         |
| [padding-left](https://www.runoob.com/cssref/pr-padding-left.html) | 设置元素的左部填充                         |
| [padding-right](https://www.runoob.com/cssref/pr-padding-right.html) | 设置元素的右部填充                         |
| [padding-top](https://www.runoob.com/cssref/pr-padding-top.html) | 设置元素的顶部填充                         |

##  9. Dimension (尺寸)属性

| 属性                                                         | 描述                 |      |
| :----------------------------------------------------------- | :------------------- | ---- |
| [height](https://www.runoob.com/cssref/pr-dim-height.html)   | 设置元素的高度。     |      |
| [line-height](https://www.runoob.com/cssref/pr-dim-line-height.html) | 设置行高。           |      |
| [max-height](https://www.runoob.com/cssref/pr-dim-max-height.html) | 设置元素的最大高度。 |      |
| [max-width](https://www.runoob.com/cssref/pr-dim-max-width.html) | 设置元素的最大宽度。 |      |
| [min-height](https://www.runoob.com/cssref/pr-dim-min-height.html) | 设置元素的最小高度。 |      |
| [min-width](https://www.runoob.com/cssref/pr-dim-min-width.html) | 设置元素的最小宽度。 |      |
| [width](https://www.runoob.com/cssref/pr-dim-width.html)     | 设置元素的宽度。     |      |

