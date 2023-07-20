

# 1. HTML基础

超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。

[HTML简介](https://www.runoob.com/html/html-intro.html)

## 1.1 标签语法

| 单标签   | 双标签                          |
| -------- | ------------------------------- |
| 成对出现 | 只有开始标签没有结束标签        |
|          | 1. 换行为：<br> 2. 水平线：<hr> |

## 1.2 HTML基本骨架

>+ html:整个网页
>
>>+ head：网页的头部
>>  + title
>>
>>+ body：网页的主体
>>
>>
>
>

## 1.3 标签的关系

+ 父子关系（嵌套关系）

  + ~~~ html
    <html>
        <head>
            
        </head>
    </html>
    
    
    
    ~~~

  + 代码格式：子级标签换行且缩进（Tab）

+ 兄弟关系（并列关系）

  + ~~~html
    <head></head>
    <body></body>
    ~~~

  + 代码格式：兄弟标签换行对齐

## 1.4 注释

~~~ html
在VS code 中注释的快捷键为 ：Ctrl + /
<!-- 这个是注释 -->
~~~

## 1.5 标题标签

~~~html
<h1></h1> 一般只用一次
<h2></h2>
一共有六个级别
~~~

## 1.6 段落标签

~~~html
<p></p>
<p></p>
~~~

**显示特点：**

+ 独占一行
+ 双标签
+ 段落间存在间隙

## 1.7 换行和水平标签

+ 换行：单标签<br>

  +  ~~~html
    <br> 浏览器不识别Enter键换行
    ~~~

+ 水平线：单标签<hr>

  + ~~~html
    <hr>
    ~~~

## 1.8 文本格式化标签

为文本添加特定格式，以突出重点

| 标签名（强调含义的标签）重点 | 效果          | 标签名 | 效果          |
| ---------------------------- | ------------- | ------ | ------------- |
| strong                       | **加粗**      | b      | **加粗**      |
| em                           | *倾斜*        | *i*    | *倾斜*        |
| ins                          | <u>下划线</u> | u      | <u>下划线</u> |
| del                          | ~~删除线~~    | s      | ~~删除线~~    |

## 1.9 图像标签

**作用：**在网页上插入图片

~~~html
<img src="图片的URL">不换行
<img src=".\cat,jpg">不换行
src用于指定图像的位置和名称，是<img>标签的必须属性
~~~

**图片标签属性**

| 标号 | 属性        | 值                                 | 描述                                         |
| ---- | ----------- | ---------------------------------- | -------------------------------------------- |
| 1    | alt         | *text*                             | 规定图像的替代文本。                         |
| 2    | src         | *URL*                              | 指定显示图像的 URL。                         |
| 3    | width       | *px(pixels)、%*                    | 设置图像的宽度（像素或百分比）。             |
| 4    | height      | *pixels*                           | 定义图像的高度（像素或百分比）。             |
| 5    | ismap       | ismap                              | 将图像定义为服务器端图像映射。               |
| 6    | usemap      | #*mapname*                         | 将图像定义为客户器端图像映射。               |
| 7    | loading     | eager：立即加载<br/>lazy：延迟加载 | 指定浏览器是应立即加载图像还是延迟加载图像。 |
| 8    | crossorigin | anonymous<br/>use-credentials      | 设置图像的跨域属性                           |

[HTML全局属性](https://www.runoob.com/tags/ref-standardattributes.html)

## 1.10 路径

+ 绝对路径：从当前位置出发查找目标文件
+ 绝对路径：从盘符出发查找目标文件（Windows 电脑从盘符出发）
+ windows 默认是\,其他系统是/，建议统一写成/

~~~ 
/表示进入某个文件夹里面
.表示当前文件所在位置
..表示到上级文件夹
~~~

## 1.11 超链接

[超链接标签详解](###7. 链接)

## 1.12 多媒体标签

[多媒体标签详解](### 6. Audio/Video)

## 1.13 列表 

[列表标签详解](###8. 列表)

[列表](https://www.runoob.com/html/html-lists.html)

列表 表格 表单都是嵌套

列表

**作用：**布局内容排列整齐的区域

**列表分类：**

+ 无序列表

  + ~~~ html
    ul嵌套li,ul是无序列表，li是列表条目
    ul标签只能包含li
    li标签内容可以是任何内容
    <ul>
        <li></li>
        <li></li>
    </ul>
    ~~~

+ 有序列表

  + ~~~html
    ol嵌套li,ol是有序列表，li是列表条目
    ol标签只能包含li
    li标签内容可以是任何内容
    <ol>
        <li></li>
        <li></li>
    </ol>
    ~~~

+ 定义列表

  + ~~~html
    dl嵌套dt和dd,dt是定义列表的标题，dd是定义列表的描述/详情
    dl里面只能放dt,dd
    dd,dt可以放任何内容
    <dl>
        <dt>标题</dt>
        <dd></dd>
        <dd></dd>
        <dd></dd>
    </dl>
    ~~~

## 1.14 表格

[表格标签详解](###9. 表格)

[表格](https://www.runoob.com/html/html-tables.html)

**标签：table嵌套tr , tr嵌套td/th**

| 标签名 | 说明       |
| ------ | ---------- |
| table  | 表格       |
| tr     | 行         |
| th     | 表头单元格 |
| td     | 内容单元格 |

~~~html
默认是没有边框线，使用border添加边框线
<table>
    <tr>
    	<th>男</th>
        <th>女</th>
    </tr>
    <tr>
    	<td>89</td>
        <td>90</td>
    </tr>
    <tr>
    	<td>89</td>
        <td>90</td>
    </tr>
</table>
~~~

**合并单元格**

~~~html
保留左上的单元格
<table>
    <tr>
    	<th>男</th>
        <th>女</th>
    </tr>
    <tr>
    	<td rowspan="2">89</td>跨行合并
        <td>90</td>
    </tr>
    <tr>
    	
        <td>90</td>
    <tr>
    	<td colspan="2">89</td>跨列合并
        
    </tr>
    </tr>
</table>
~~~

## 1.15 表单

**作用：手机用户信息**

[\<input>标签详解](https://www.runoob.com/tags/tag-input.html)

[表单](https://www.runoob.com/html/html-forms.html)

+ \<input>标签

+ 下拉菜单

+ 文本域

+ label标签

  + ~~~html
    <label><input type="radio"></label>
    <input type="radio" id="man">
    <label for="man"></label>
    ~~~

+ 按钮

[合并单元格属性](https://www.runoob.com/tags/tag-td.html)

## 1.16 HTML 区块

**HTML \<div> 和\<span>**

[HTML <div> 和<span>](https://www.runoob.com/html/html-blocks.html)

## 1.17 字符实体

HTML 中的预留字符必须被替换为字符实体。

一些在键盘上找不到的字符也可以使用字符实体来替换。

+++



[字符实体](https://www.runoob.com/html/html-entities.html)

## 案例

### 案例一 -个人简历

### 案例二 -Vue简介

### 案例一--体育新闻列表

### 案例二-注册信息



# 2. HTML的详细用法

## 2.1 所有标签（按功能分类）

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

## 2.2 全局属性

| 属性                                                         | 描述                                                       |
| :----------------------------------------------------------- | :--------------------------------------------------------- |
| [accesskey](https://www.runoob.com/tags/att-global-accesskey.html) | 设置访问元素的键盘快捷键。                                 |
| [class](https://www.runoob.com/tags/att-global-class.html)   | 规定元素的类名（classname）                                |
| [contenteditable](https://www.runoob.com/tags/att-global-contenteditable.html)**New** | 规定是否可编辑元素的内容。                                 |
| [contextmenu](https://www.runoob.com/tags/att-global-contextmenu.html)**New** | 指定一个元素的上下文菜单。当用户右击该元素，出现上下文菜单 |
| [data-*](https://www.runoob.com/tags/att-global-data.html)**New** | 用于存储页面的自定义数据                                   |
| [dir](https://www.runoob.com/tags/att-global-dir.html)       | 设置元素中内容的文本方向。                                 |
| [draggable](https://www.runoob.com/tags/att-global-draggable.html)**New** | 指定某个元素是否可以拖动                                   |
| [dropzone](https://www.runoob.com/tags/att-global-dropzone.html)**New** | 指定是否将数据复制，移动，或链接，或删除                   |
| [hidden](https://www.runoob.com/tags/att-global-hidden.html)**New** | hidden 属性规定对元素进行隐藏。                            |
| [id](https://www.runoob.com/tags/att-global-id.html)         | 规定元素的唯一 id                                          |
| [lang](https://www.runoob.com/tags/att-global-lang.html)     | 设置元素中内容的语言代码。                                 |
| [spellcheck](https://www.runoob.com/tags/att-global-spellcheck.html)**New** | 检测元素是否拼写错误                                       |
| [style](https://www.runoob.com/tags/att-global-style.html)   | 规定元素的行内样式（inline style）                         |
| [tabindex](https://www.runoob.com/tags/att-global-tabindex.html) | 设置元素的 Tab 键控制次序。                                |
| [title](https://www.runoob.com/tags/att-global-title.html)   | 规定元素的额外信息（可在工具提示中显示）                   |
| [translate](https://www.runoob.com/tags/att-global-translate.html)**New** | 指定是否一个元素的值在页面载入时是否需要翻译               |

### 2.3 事件

## 2.1 \<head>标签

[\<head> 标签](https://www.runoob.com/tags/tag-head.html)

### 2.1.1 代码实例

**一份在头部带有 \<title> 标签的 HTML 文档：**

~~~html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>文档标题</title>
</head>
 
<body>
文档内容......
</body>
 
</html>
~~~

### 2.1.2 标签定义及使用说明

\<head> 元素是所有头部元素的容器。

\<head> 元素必须包含文档的标题（title），可以包含脚本、样式、meta 信息 以及其他更多的信息。

以下列出的元素能被用在\<head> 元素内部：

- [title](https://www.runoob.com/tags/tag-title.html) （在头部中，这个元素是必需的）
- [style](https://www.runoob.com/tags/tag-style.html)
- [base](https://www.runoob.com/tags/tag-base.html)
- [link](https://www.runoob.com/tags/tag-link.html)
- [meta](https://www.runoob.com/tags/tag-meta.html)
- [script](https://www.runoob.com/tags/tag-script.html)
- [noscript](https://www.runoob.com/tags/tag-noscript.html)

### 2.1.3 全局属性

**\<head>标签支持**：[HTML 的全局属性](https://www.runoob.com/tags/ref-standardattributes.html)

## 2.2  \<body> 标签

**一个简单的 HTML 文档，包含尽可能少的必需的标签：**

~~~html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>文档标题</title>
</head>
 
<body>
文档内容......
</body>
 
</html>
~~~



# 3. 全局属性

[HTML全局属性](https://www.runoob.com/tags/ref-standardattributes.html)