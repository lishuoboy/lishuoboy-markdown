教程和实例在我的有道云笔记

其它菜鸟教程  https://www.runoob.com/markdown/md-tutorial.html

实例已放入码云：https://gitee.com/lishuoboy/lishuoboy-markdown

# 1.目录(IDEA、有道不支持)

@[toc]

# 2.标题

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

# 3. 文本样式

> 引用

**加粗**

*斜体*

~~删除线~~

<u>下划线2</u>

++下划线（IDEA、Typora、CSDN不支持）++

==标记黄底（IDEA、Typora不支持）==

下标 H~2~O（IDEA、Typora不支持）

上标 2^10^（IDEA、Typora不支持）

# 4.列表

## 有序列表

1. 一级
    1. 二级
        1. 三级
2. 一级

## 无序列表

- 一级
    - 二级
        - 三级
- 一级
    + 二级
        + 三级

## 任务列表

- [x] 完成任务列表
- [x] 完成任务列表
- [ ] 未完成任务列表
- [ ] 未完成任务列表

## 自定义列表（IDEA、Typora不支持）

Markdown
:  Text-to-HTML conversion tool

Authors
:  John
:  Luke

# 5.超链接

[超链接](https://www.baidu.com)

# 6.图片

图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw)

下面带格式的图片（IDEA、Typora、有道不支持） 带尺寸的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw =30x30)

宽度确定高度等比例的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw =30x)

高度确定宽度等比例的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw =x30)

居中的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw#pic_center)

居中并且带尺寸的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw#pic_center=30x30)

居右的图片:
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw#pic_right)

# 7.水平线

---

# 8.表格

| 序号  | 姓名  |
|-----|-----|
| 1   | 张三  |
| 2   | 李四  |

# 9. HTML

<html lang="zh">
<!-- 在这里插入内容 -->
<b>html内容</b>
</html>

# 10.各种代码片

## 10.1. java/javascript

```java
/** 注释 */
public class User {
    private String name;  // 姓名
}
```

```javascript
/** 注释 */
function getName() {
    return "张三";  // 姓名
}
```

## 10.2. JSON/XML

```json
{
  "id": 1,
  "name": "张三"
}
```

```xml

<root>
    <id>1</id>
    <name>张三</name>
</root>
```

## 10.3 公式（IDEA、有道云不支持）

$$ E = mc^2 $$

Gamma公式展示 $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ 是通过 Euler integral

$$ \Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,. $$

## 10.3 math（IDEA、Typora、CSDN不支持）

```math
E = mc^2
```

```math
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,. 
```

## 10.4 graph 流程图（都支持，但是有道不能有mermaid）

```mermaid
graph LR
A -->B
```

```mermaid
graph LR
A[长方形] -- 链接 --> B((圆))
A --> C(圆角长方形)
B --> D{菱形}
C --> D
```

## 10.5 mermaid 流程图（IDEA、Typora、有道不支持）

```mermaid
flowchat
st=>start: 开始
e=>end: 结束
op=>operation: 我的操作
cond=>condition: 确认？

st->op->cond
cond(yes)->e
cond(no)->op
```

## 10.6 UML时序图（IDEA不支持，有道支持但是不能有mermaid）

```mermaid
sequenceDiagram
A->>B: How are you?
B->>A: Great!
```

```mermaid
sequenceDiagram
张三 ->> 李四: 你好！李四, 最近怎么样?
李四-->>王五: 你最近怎么样，王五？
李四--x 张三: 我很好，谢谢!
李四-x 王五: 我很好，谢谢!
Note right of 王五: 李四想了很长时间, 文字太长了<br/>不适合放在一行.

李四-->>张三: 打量着王五...
张三->>王五: 很好... 王五, 你怎么样?
```

## 10.6 甘特图（IDEA不支持，有道支持但是不能有mermaid）

```mermaid
gantt
dateFormat YYYY-MM-DD
section S1
T1: 2014-01-01, 9d
section S2
T2: 2014-01-11, 9d
section S3
T3: 2014-01-02, 9d

```

```mermaid
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section 现有任务
        已完成               :done,    des1, 2014-01-06,2014-01-08
        进行中               :active,  des2, 2014-01-09, 3d
        计划中               :         des3, after des2, 5d
```

## 10.7 类图（IDEA、Typora、有道不支持）

```mermaid
classDiagram
    Class01 <|-- AveryLongClass : Cool
    <<interface>> Class01
    Class09 --> C2 : Where am i?
    Class09 --* C3
    Class09 --|> Class07
    Class07 : equals()
    Class07 : Object[] elementData
    Class01 : size()
    Class01 : int chimp
    Class01 : int gorilla
    class Class10 {
        >>service>>
        int id
        size()
    }
```

# 11. 脚注

引用URL。[^1]

引用本地文件。[^2]

[^1]: http://www.baidu.com

[^2]: .gitignore
