# markdown-handbook
:kissing:Markdown 简明语法手册:kissing:

---
## <a name="index"/>目录
* [标题](#title)
* [文本](#text)
    * 普通文本
    * 单行文本
    * 多行文本
    * 文字高亮
* [横线](#line)
* [链接](#link) 
    * 文字超链接
    *  锚点
    * 图片超链接
* [图片](#pic)
* [列表](#dot)
    * 圆点列表
    * 数字列表
    * 复选框列表
* [块引用](#blockquotes)
* [代码](#code)
* [表格](#table) 
* [表情](#emoji)

***

### <a name="title"/> 1.标题

行首加井号表示不同级别的标题 (H1-H6),例如：# H1, ## H2, ### H3，#### H4.

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

***

 也可以使用在文字下放加 === 表示一级标题,使用 --- 表示二级标题. 

一级标题
====

二级标题
---

### 2. 文本 <a name="text"/>
+ 普通文本

 直接输入的文字就是普通文本。需要注意的是要换行的时候不<br>能直接通过回车来换行，需要使用\<br\>.也就是html里面的标签. 注意第三行的`<br>`前加了反斜杠 \\ .目的就是像其他语言那样实现转义，也就是 \<  的转义.
 
+ 单行文本

        使用两个Tab符实现单行文本.
+ 多行文本

        多行文本和
        单行文本异曲同工，只要在
        每行行首加两个Tab.
+ 文字高亮

如果你想使一段话中部分文字高亮显示，来起到突出强调的作用，那么可以把它用 \`  \` 包围起来.`注意`这不是单引号，而是`Tab`上方，`数字1`左边的按键（注意使用`英文`输入法).
        
### 3. 斜体和粗体

使用 * 和 ** 表示斜体和粗体.

这是 *斜体*,这是 **粗体**.

### 4. 删除线

~~使用\~\~表示删除线.~~

### 5. 外链接<a name="link"/>

使用 \[描述](链接地址) 为文字增加外链接。

这是去往 [有趣的HTML5和CSS3特效在线演示地址](http://gnipbao.github.io/css3-test/menu.html) 的链接。

### 6.锚点<a name=""/>
我们可以使用HTML的锚点标签（`#`）来设置锚点：[回到目录](#index)  
但其实呢，每一个标题都是一个锚点，不需要用标签来指定，比如我们 [回到顶部](#TEST)
不过不幸的是，由于对中文支持的不好，所以中文标题貌似是不能视作标签的。

### <a name="dot"/> 6. 列表

使用 *，+，- 表示无序列表。

- 无序列表项 一
- 无序列表项 二
- 无序列表项 三

二级三级原点

+ 编程语言
    + 脚本语言
        + Python

使用数字和点表示有序列表。

1. 有序列表项 一
2. 有序列表项 二
3. 有序列表项 三

### 7. 数字列表自动排序
也可以在第一行指定`1. `，而接下来的几行用星号`*`（或者继续用数字1. ）就可以了，它会自动显示成2、3、4……    
面向对象的七大原则：
      
1. 开闭原则
* 里氏转换原则
* 依赖倒转原则
1. 接口隔离原则
1. 组合聚合复用原则
1. 迪米特法则
1. 单一直则原则 
    
### 8. 多级数字列表
和圆点的列表一样，数字列表也有多级结构：  

1. 这是一级的数字列表，数字1还是1
   1. 这是二级的数字列表，阿拉伯数字在显示的时候变成了罗马数字
      1. 这是三级的数字列表，数字在显示的时候变成了英文字母
	    1. 四级的数字列表显示效果，就不再变化了，依旧是英文字母

### 9. 复选框列表
- [x] C
- [x] C++
- [x] Java
- [x] Qt
- [x] Android
- [ ] C#
- [ ] .NET

### 10. 文字引用

使用 > 表示文字引用。

单个引用：

> 野火烧不尽，春风吹又生。

字符包围：

> 数据结构
>> 树
>>> 二叉树
>>>> 平衡二叉树
>>>>> 满二叉树

### 11. 代码块<a name="blockquotes"/>

使用 四个缩进空格 表示代码块。

示例：

    这是一个代码块，此行左侧有四个不可见的空格。

### 12. 加强的代码块 <a name="code"/>

支持四十一种编程语言的语法高亮的显示，行号显示。

非代码示例：

```
$ sudo npm install 
```

Python 示例：

```python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None

class SomeClass:
    pass

>>> message = '''interpreter
... prompt'''
```

JavaScript 示例：

``` javascript
/**
* nth element in the fibonacci series.
* @param n >= 0
* @return the nth element, >= 0.
*/
function fib(n) {
  var a = 1, b = 1;
  var tmp;
  while (--n >= 0) {
    tmp = a;
    a += b;
    b = tmp;
  }
  return a;
}

document.write(fib(10));
```


### <a name="pic"/> 13.插入图像

使用 \!\[描述](图片链接地址) 插入图像。

插入图片示例：

![Markdown](https://github.com/gnipbao/gnipbao.github.io/blob/master/images/markdown.jpg)

给图片添加链接:

[![V]](http://gnipbao.github.io/css3-test/src/Funny-demo/Button/index.html)
[V]:https://github.com/gnipbao/gnipbao.github.io/blob/master/images/markdown.jpg

### <a name="table"/>14.显示表格
    表头1  | 表头2
    ------------- | -------------
    Content Cell  | Content Cell
    Content Cell  | Content Cell
    
|表头1  | 表头2           |		
|------------- | -------------| 
|Content Cell  | Content Cell | 
|Content Cell  | Content Cell | 
    
|名字 | 描述          
|------------- | -----------| 
|Help      | Display the help window.|
|Close     | Closes a window |    
    
表格中也可以使用普通文本的删除线，斜体等效果
    
| 名字 | 描述          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |
    
表格可以指定对齐方式
    
| 左对齐 | 居中  | 右对齐 |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
    
表格中嵌入图片

| 图片 | 描述 |
| ---- | ---- |
![Markdown](https://github.com/gnipbao/gnipbao.github.io/blob/master/images/markdown.jpg) |图片


### 15. Html 标签

本站支持在 Markdown 语法中嵌套 Html 标签，譬如，你可以用 Html 写一个纵跨两行的表格：

    <table>
        <tr>
            <th rowspan="2">值班人员</th>
            <th>星期一</th>
            <th>星期二</th>
            <th>星期三</th>
        </tr>
        <tr>
            <td>李强</td>
            <td>张明</td>
            <td>王平</td>
        </tr>
    </table>

<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>

### 16. 待办事宜 Todo 列表

使用带有 [ ] 或 [x] （未完成或已完成）项的列表语法撰写一个待办事宜列表，并且支持子列表嵌套以及混用Markdown语法，例如：

    - [ ] **Cmd Markdown 开发**
        - [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
        - [ ] 支持以 PDF 格式导出文稿
        - [x] 新增Todo列表功能 
        - [x] 改进 LaTex 功能
            - [x] 修复 LaTex 公式渲染问题
            - [x] 新增 LaTex 公式编号功能 
    - [ ] **七月旅行准备**
        - [ ] 准备邮轮上需要携带的物品
        - [ ] 浏览日本免税店的物品
        - [x] 购买蓝宝石公主号七月一日的船票
        
对应显示如下待办事宜 Todo 列表：
        
- [ ] **Cmd Markdown 开发**
    - [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
    - [ ] 支持以 PDF 格式导出文稿
    - [x] 新增Todo列表功能 
    - [x] 改进 LaTex 功能
        - [x] 修复 LaTex 公式渲染问题
        - [x] 新增 LaTex 公式编号功能 
- [ ] **七月旅行准备**
    - [ ] 准备邮轮上需要携带的物品
    - [ ] 浏览日本免税店的物品
    - [x] 购买蓝宝石公主号七月一日的船票

#### <a name="emoji"/>17.添加表情
Github的Markdown语法支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情.

比如`:blush:`，可以显示:blush:.

详细查看[emoji](./emoji.md).
        
        
