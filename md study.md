# Markdown 标题

# 一级标题  

"#"

## 二级标题

“##”

# Markdown 段落格式

first   



second

## 字体

*斜体*     "*  *"

_斜体_     “_    _”

**粗体**    "**   **"

__粗体__     “__    __”

***粗斜体***   “3*   3*”

___粗斜体___   “3_    3_”

## 分割线

今天是2021/22/04   "***"

***

今天是2021/22/04   "---"

---

## 删除线

~~2021/11/04~~

"~~    ~~"

## 下划线

<u>下划线</u>

"<u></u>"

## 脚注

今天是[^2021/11/04]

[^2021/11/04]:今天的日期

 

# Markdown列表

## 无序列表

* 第一项

* 第二项

* 第三项

  “* ”

***

+ 第一项

+ 第二项

+ 第三项

   “+ ”

---

- 第一项

- 第二项

- 第三项
  “- ”

## 有序列表

1. 第一项
2. 第二项
3. 第三项

“数字+ . +空格符”

## 列表嵌套

1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
    

# Markdown区块

> 区块引用
>
> > 第一区块
> >
> > > 第二区块

“>   >>   >>>”

## 区块中使用列表

> 区块
>
> 1. 第一项
> 2. 第二项
>
> + 第一项
> + 第二项

"先区块再插入列表"

## 列表中使用区块

* 第一项

  > 2021/11/05
  >
  > 11:08

* 第二项

“先列表再插入区块”

# Markdown代码

`printf()`函数

## 代码区块

​	<?java

​		printf("hello!");

````java
int s;
int a = 1,b = 2;
s = a + b;
printf("%d", s);
````

# Markdown链接

这是一个链接[菜鸟教程](http://www.runoob.com)

"[链接名称]（链接地址）"

<http://www.runoob.com>

"<链接名称>"

## 高级链接

这个链接用1108作为网址变量[百度][1108]

这个链接用runoob作为网址变量[Runoob][runoob]

在文档的结尾为变量赋值（网址）

[1108]:http://www.baidu.com/
[runoob]:http://www.runoob.com/

”[内容] [变量]

[变量] :网址“

# Markdown 图片

! [RUNOOB 图标] (http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

! [RUNOOB 图标] (http://static.runoob.com/images/runoob-logo.png "RUNOOB")

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

"![图片的代替文字] (图片网址 ”选择性的’title‘属性的文字“)"



这个链接用1511作为网址变量[Runoob][1511]

在文档的结尾为变量赋值（网址）

[1511]:http://static.runoob.com/images/runoob-logo.png



使用<img>标签对图片大小进行改变

< img src="http://static.runoob.com/images/runoob-logo.png" width="30%" >

<img src="http://static.runoob.com/images/runoob-logo.png" width="30%">
