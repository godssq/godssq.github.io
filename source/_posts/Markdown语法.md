---
title: Markdown语法
date: 2021-09-25 22:10:44
tags:
---

# Markdown

Markdown是一种纯文本格式的标记语言。通过简单的标记语法，它可以使普通文本内容具有一定的格式。



**标题语法**

在单词或短语前面添加井号 (`#`) 。`#` 的数量代表了标题的级别。例如，添加三个 `#` 表示创建一个三级标题 ，以此类推。需要注意的是在“#”后需添加一个空格。



**段落语法**

1.创建段落，使用空白行将一行或多行文本进行分割。

2.在一行的末尾添加两个或多个空格，然后按回车键。



**字体**

1.粗体：在单词或短语的前后各添加两个星号，如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号。

eg：**粗体**

2.斜体：在单词或短语前后添加一个星号，要**斜体突出单词的中间部分**，请在字母前后各添加一个星号，**中间不要带空格**。

eg：*斜体*

3.粗体&斜体：要同时用粗体和斜体突出显示文本，在单词或短语的前后各添加三个星号，要**加粗并用斜体显示单词或短语的中间部分**，请在要突出显示的部分前后各添加三个星号，**中间不要带空格**。

eg：***粗体&斜体***



**引用语法**

1.创建块引用，在段落前增加一个 `>` 符号

eg：>	我今天好帅啊

渲染效果如下：

> 我今天好帅啊

2.多个段落的块引用：

eg：> 我今天

​		> 好帅啊

渲染效果如下：

> 我今天
>
> 好帅啊

3.嵌套快引用：

eg：>我今天

​		>>好帅啊

渲染效果如下：

> 我今天
>
> > 好帅啊

4.带有其他元素块的引用：

块引用可以包含其他 Markdown 格式的元素，但 并非所有元素都可以使用，需要进行实验以查看哪些元素有效。

eg：> ### 我

​		> - 今天

​		>  - 好帅

​		> \*啊*

渲染效果如下：

> ###我
>
> - 今天
>
> - 好帅
>
>   *啊*



**列表语法**

1.有序列表：要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

eg：1.

​		2.

2.无序列表：要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

eg：-	First item

​		-	Second item

预览效果如下：

- First item
- Second item

3.在列表中嵌套其他元素：要在保留列表连续性的同时在列表中添加另一种元素，需将该元素缩进四个空格或一个制表符。

eg：*	我

​		*	今天

​				好帅

​		*	啊

渲染效果如下：

* 我

* 今天

  好帅

* 啊

4.引用块

eg：*	我

​		*	今天

​				>	好帅

​		*	啊

渲染效果如下：

* 我

* 今天

  > 好帅

* 啊

5.代码块：代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，需将它们缩进八个空格或两个制表符。

eg：1.Open the file.

​		2.Find the following code block on line 21:

​				<html>

​					<head>

​						<title>Test</title>

​					</head>

​		3.Update the title to match the name of your website.

渲染效果如下：

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website

6.列表

eg：

1. First item

2. Second item

3. Third item

    -Indented item

    -Indented item

4. Fourth item

渲染效果如下：

1. First item

2. Second item

3. Third item

   - Indented item

   - Indented item

4. Fourth item



**代码语法**

1、转移反引号：要将单词或短语表示为代码，请将其包裹在反引号 (`) 中。

eg:	At the command prompt,type `nano`. 

2、代码块：要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

eg：

```text
	<html>
      <head>
      </head>
    </html>
```



**分割线语法**

要创建分隔线，请在单独一行上使用三个或多个星号 (*)、破折号 (-) 或下划线 (_) ，并且不能包含其他内容。一般会在分割线的前后均添加空白行。

eg：

三个星号*：

***

三个破折号-：

---

三个下划线_：

___



**链接语法**

1、链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

eg：[Markdown语法](https://markdown.com.cn/basic-syntax/links.html "Markdown官方教程")

点击方法：Ctrl+Click

2、网址和Email地址：使用尖括号URL或者email地址变成可点击的链接。

eg：<https://markdown.com.cn>

<fake@example.com>

3、带格式化的链接：强调链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

eg：**[Markdown](https://markdown.com.cn/basic-syntax/links.html)**

*[Markdown](https://markdown.com.cn/basic-syntax/links.html)*

**[`Markdown`](https://markdown.com.cn/basic-syntax/links.html)**



**图片语法**

要添加图像，请使用感叹号 (`!`), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。

1、上传网络图

语法：![图片 alt ] (图片链接地址)
（图片 alt 为用来描述图片的关键词，可以不写。）

2、上传本地图片

打开刚才创建的 [XXX.md](http://xxx.md/) 文件

将 /blog/source/_post/XXX/Test.jpg 直接拖拽到 Typora 编辑界面

会自动连带图片生成：

```
![1](D:\blog\source\_posts\re\1.png)
```

将就绝对路径删除部分，仅保留：

```
![1-Image](re\1.png)
```

若挪开选中图片的鼠标，自动隐藏引用代码，仅将图片显示

然后直接上传到Github即可。
