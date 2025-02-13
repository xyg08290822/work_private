# Markdown学习文档

## 一、标题

在Markdown中，有两种方式可以创建标题，一种是使用`#`符号，另一种是使用`=`和`-`符号。

### 1. 使用`#`符号

在Markdown中，可以使用`#`符号来创建标题。`#`符号后面可以跟一个空格，然后输入标题的文本。`#`符号的数量表示标题的级别，最多支持6级标题。

例如：

```text
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

### 2. 使用`=`和`-`符号

在Markdown中，可以使用`=`和`-`符号来创建标题。`=`符号后面可以跟一个空格，然后输入标题的文本。`-`符号后面可以跟一个空格，然后输入标题的文本。

例如：

```text
一级标题
=================

二级标题
-----------------
```

## 二、段落

在Markdown中，段落是由一个或多个连续的文本行组成，每行的开头不能有缩进。段落之间用空行分隔。

例如：

```text
这是第一段。

这是第二段。
```

## 三、换行

在Markdown中，可以使用两个空格加回车来创建换行。

例如：

```text
这是第一行。
这是第二行。
```

## 四、粗体和斜体

在Markdown中，可以使用`*`或`_`符号来创建粗体和斜体文本。

### 1. 粗体

在Markdown中，可以使用两个`*`或两个`_`符号来创建粗体文本。

例如：

```text
这是**粗体文本**。
```

### 2. 斜体

在Markdown中，可以使用一个`*`或一个`_`符号来创建斜体文本。

例如：

```text
这是*斜体文本*。
```

## 五、引用

在Markdown中，可以使用`>`符号来创建引用文本。

例如：

```text
> 这是一个引用文本。
```

## 六、代码

在Markdown中，可以使用反引号（`）来创建行内代码和代码块。

### 1. 行内代码

在Markdown中，可以使用一个反引号（`）来创建行内代码。

例如：

```text
这是`行内代码`。
```

### 2. 代码块

在Markdown中，可以使用三个反引号（```）来创建代码块。

例如：

~~~text
```python
print("Hello, World!")
``` {data-source-line="86"}
~~~

## 七、链接

在Markdown中，可以使用`[]`和`()`来创建链接。

例如：

```text
这是一个[链接](https://www.example.com)。
```

## 八、图片

在Markdown中，可以使用`![]()`来创建图片。

例如：

```text
![图片描述](https://www.example.com/image.jpg)
```

## 九、列表

在Markdown中，可以使用`*`、`+`或`-`符号来创建无序列表，使用数字和`.`符号来创建有序列表。

### 1. 无序列表

在Markdown中，可以使用`*`、`+`或`-`符号来创建无序列表。

例如：

```text
- 列表项1
- 列表项2
- 列表项3
```

### 2. 有序列表

在Markdown中，可以使用数字和`.`符号来创建有序列表。

例如：

```text
1. 列表项1
2. 列表项2
3. 列表项3
```

## 十、表格

在Markdown中，可以使用`|`符号来创建表格。

例如：

```text
| 姓名 | 年龄 | 性别 |
| ---- | ---- | ---- |
| 张三 | 20   | 男   |
| 李四 | 22   | 女   |
| 王五 | 25   | 男   |
```

## 十一、分割线

在Markdown中，可以使用三个`-`符号来创建分割线。

例如：

```text
---
```

## 十二、转义字符

在Markdown中，可以使用`\`符号来转义特殊字符。

例如：

```text
\*这是转义后的星号\*
```

## 十三、任务列表

在Markdown中，可以使用`- [ ]`或`- [x]`来创建任务列表。

例如：

```text
- [ ] 任务1
- [x] 任务2
```

## 十四、脚注

在Markdown中，可以使用`[^1]`来创建脚注。

例如：

```text
这是一个脚注[^1]。

[^1]: 这是脚注内容。
```

## 十五、数学公式

在Markdown中，可以使用`$$`符号来创建数学公式。

例如：

```text
$$  E = mc^2   $$
```

## 十六、流程图

在Markdown中，可以使用Mermaid语法来创建流程图。

例如：

~~~text
```mermaid
graph LR
A[开始] --> B{判断}
B -->|是| C[处理]
B -->|否| D[结束]
C --> E[结束]
``` {data-source-line="183"}
~~~

## 十七、时序图

在Markdown中，可以使用Mermaid语法来创建时序图。

例如：

~~~text
```mermaid
sequenceDiagram
A->>B: 你好
B->>A: 你好
``` {data-source-line="194"}
~~~

## 十八、甘特图

在Markdown中，可以使用Mermaid语法来创建甘特图。

例如：

~~~text
```mermaid
gantt
    title 甘特图示例
    dateFormat  YYYY-MM-DD
    section 项目A
    任务1: a1, 2022-01-01, 30d
    任务2: after a1, 20d
    section 项目B
    任务3: 2022-01-01, 20d
``` {data-source-line="210"}
~~~

## 十九、类图

在Markdown中，可以使用Mermaid语法来创建类图。

例如：

~~~text
```mermaid
classDiagram
    class Person {
        +String name
        +int age
        +void sayHello()
    }
    class Student {
        +String school
        +void study()
    }
    Person <|-- Student
``` {data-source-line="229"}
~~~

## 二十、UML图

在Markdown中，可以使用Mermaid语法来创建UML图。

例如：

~~~text
```mermaid
uml
    classDiagram
        class Person {
            +String name
            +int age
            +void sayHello()
        }
        class Student {
            +String school
            +void study()
        }
        Person <|-- Student
``` {data-source-line="249"}
~~~

## 二十一、饼图

在Markdown中，可以使用Mermaid语法来创建饼图。

例如：

~~~text
```mermaid
pie
    title 水果销售情况
    "苹果" : 30
    "香蕉" : 20
    "橙子" : 50
``` {data-source-line="262"}
~~~

## 二十二、雷达图

在Markdown中，可以使用Mermaid语法来创建雷达图。

例如：

~~~text
```mermaid
radar
    title 雷达图示例
    A : 2
    B : 3
    C : 4
    D : 5
    E : 6
``` {data-source-line="277"}
~~~

## 二十三、树图

在Markdown中，可以使用Mermaid语法来创建树图。

例如：

~~~text
```mermaid
tree
    root
        child1
        child2
            child2_1
            child2_2
        child3
``` {data-source-line="292"}
~~~