# Markdown-基本语法
https://markdown.com.cn/
## Markdown 基本语法

Markdown是一种轻量级标记语言，排版语法简洁，让人们更多地关注内容本身而非排版。它使用易读易写的纯文本格式编写文档，可与HTML混编，可导出 HTML、PDF 以及本身的 .md 格式的文件。因简洁、高效、易读、易写，Markdown被大量使用，如Github、Wikipedia、简书等。

在线体验一下 [Markdown在线编辑器](https://markdown.com.cn/editor/)

## Markdown 标题语法

要创建标题，请在单词或短语前面添加井号 \(`#`\) 。`#` 的数量代表了标题的级别。例如，添加三个 `#` 表示创建一个三级标题 \(`<h3>`\) \(例如：`### My Header`\)。

## Markdown 段落

要创建段落，请使用空白行将一行或多行文本进行分隔。

\(`<p></p>`\)

## Markdown 换行语法

在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行\(`<br>`\)。

推荐使用\(`<br>`\)来进行换行

## Markdown 强调语法

### 粗体（Bold）

要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。

推荐使用两个星号（asterisks）。

    **粗体**
    <strong>粗体</strong>

### 斜体（Italic）

要用斜体显示文本，请在单词或短语前后添加一个星号（asterisk）或下划线（underscore）。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。

    *斜体*
    <em>斜体</em>

### 粗体（Bold）和斜体（Italic）

要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。

    ***粗斜体***
    <strong><em>粗斜体</em></strong>

## Markdown 引用语法

要创建块引用，请在段落前添加一个 `>` 符号。

`> Dorothy followed her through many of the beautiful rooms in her castle.`

渲染效果如下：
> Dorothy followed her through many of the beautiful rooms in her castle.

### 多个段落的块引用

块引用可以包含多个段落。为段落之间的空白行添加一个 `>` 符号。

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

渲染效果如下：

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 嵌套块引用

块引用可以嵌套。在要嵌套的段落前添加一个 `>> `符号。

```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```
渲染效果如下：

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 带有其它元素的块引用

块引用可以包含其他 Markdown 格式的元素。

```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
```
渲染效果如下：
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Markdown 列表语法

可以将多个条目组织成有序或无序列表。

### 有序列表

要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

#### markdown 语法

```
1. First item
2. Second item
3. Third item
4. Fourth item 
```
渲染效果如下：
1. First item
2. Second item
3. Third item
4. Fourth item 

#### HTML 语法

```
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <li>Fourth item</li>
</ol> 
```
渲染效果如下：
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <li>Fourth item</li>
</ol> 

### 无序列表

要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。
```
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <li>Fourth item</li>
</ul> 
```

###  代码块
代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。

## Markdown 代码语法
要将单词或短语表示为代码，请将其包裹在反引号 \(`` ` ``\) 中。

### 转义反引号
如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号\(`` `ada` ``\)中。

```
``Use `code` in your Markdown file.``
```
渲染效果如下：

``Use `code` in your Markdown file.``


### 代码块

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

## Markdown 分隔线语法
要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。

```
***
---
___
```
渲染效果如下：

***
---
___

##  Markdown 链接语法

链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

对应的HTML代码：`<a href="超链接地址" title="超链接title">超链接显示名</a>`

`这是一个链接 [Markdown语法](https://markdown.com.cn)。`

渲染效果如下：

这是一个链接 [Markdown语法](https://markdown.com.cn)。

### 给链接增加 Title
链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

`这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。`

渲染效果如下：

这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

### 网址和Email地址
使用尖括号可以很方便地把URL或者email地址变成可点击的链接。
```
<https://markdown.com.cn>
<fake@example.com>
```
渲染效果如下：

<https://markdown.com.cn> <br>
<fake@example.com>

### 带格式化的链接


