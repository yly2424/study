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

# Markdown表格

**|** 来分隔不同的单元格，使用 **-** 来分隔表头和其他行。

|   1    |   2    |
|  ----  |  ----  |
|单元格|单元格|
|单元格|单元格|

-: 居右对齐				:- 居左对齐				:-: 居中对齐

|左对齐         |   居中对齐    |        右对齐 |
|:-----             |       :-----:        |             -----:|
|单元格         |     单元格      |         单元格|
|单元格         |     单元格      |         单元格|

# Markdown高级技巧

## 支持HTML元素

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>`等 

## 转义

Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：

**文本加粗** 

\*\* 正常显示星号 \*\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号:

"\\\"反斜线	"`"反引号	“*”星号	"_"下划线	"{ }"花括号	"[ ]"方括号

"()"小括号	"#"井字号	"+"加号	"-"减号		"."英文句点	"!"感叹号



# Typora画流程图

## 横向流程图

````mermaid
graph LR
H[横向流程图]
A(开始) -->B[处理]
B --> C{条件a}
C --> |a=1| D[结果1]
C --> |a=2| E[结果2]
D --> F[输出]
E --> F[输出]
F --> G(结束)
````





## 竖向流程图

```mermaid
graph TD
H[竖向流程图]
A(开始) -->B[处理]
B --> C{条件a}
C --> |a=1| D[结果1]
C --> |a=2| E[结果2]
D --> F[输出]
E --> F[输出]
F --> G(结束)

```

## 标准流程图

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```

## 标准流程图（横向）

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st(right)->op(right)->cond
cond(yes)->io(bottom)->e
cond(no)->sub1(right)->op
```



## UML时序图

```sequence
Title:简单使用
A -> B:B你好吗？(请求)
Note right of B:B的描述
Note left of A:A的描述
B --> A:我很好(响应)
A -> B:你真的好吗？
```

-> 直线实箭头，--> 虚线实箭头，->> 实线箭头，-->> 虚线箭头

## UML时序图（复杂）

```sequence
Title:复杂使用
A -> B:B你好吗？(请求)
Note right of B:B的描述
Note left of A:A的描述(提示)
B --> A:我很好(响应)
B -> C:你好吗？
C -->> A:B来找我了
A -> B:你真的好吗？
Note over B,C:我们是朋友
participant C
Note right of D:没人跟我玩
```



## UML标准时序图

```mermaid
%% 时序图例子,-> 直线，-->虚线，->>实线箭头
  sequenceDiagram
    participant 张三
    participant 李四
    participant 王五
    张三 ->> 王五: 王五你好吗？
    loop 健康检查
        王五 -> 王五: 与疾病战斗
    end
    Note right of 王五: 合理 食物 <br/>看医生...
    李四 -->> 张三: 很好!
    王五 ->> 李四: 你怎么样?
    李四 -->> 王五: 很好!
```



## 甘特图

```mermaid
%% 语法示例
        %% 语法示例
        gantt
        dateFormat  YYYY-MM-DD
        title 软件开发甘特图
        section 设计
        需求                      :done,    des1, 2014-01-06,2014-01-08
        原型                      :active,  des2, 2014-01-09, 3d
        UI设计                     :         des3, after des2, 5d
    	未来任务                     :         des4, after des3, 5d
        section 开发
        学习准备理解需求                      :crit, done, 2014-01-06,24h
        设计框架                             :crit, done, after des2, 2d
        开发                                 :crit, active, 3d
        未来任务                              :crit, 5d
        耍                                   :2d
        section 测试
        功能测试                              :active, a1, after des3, 3d
        压力测试                               :after a1  , 20h
        测试报告                               : 48h
```
