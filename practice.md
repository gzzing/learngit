---

---



# How to use

Thank you for choosing **Typora** 

## Live Preview

**Typora** use the feature: *Live Preview*, meaning that you could see these inline styles after you finish typing, and see block styles when you type or after you press `Enter` key or focus another paragraph

- Select word H~2~O and 2^12^ 
- Delete word: 
- cmd +/-
- this

## Pandoc

[Pandoc](http://pandoc.org/) 是一个通用文档转化器。

### 安装Pandoc

- homebrew


- 官网下载安装包



## 块级元素

### 段落和换行

段落是一行或多行连续的文本。在Markdown中段落由超过一行的空行分割。

在Typora中，你只需要按下 `Return` 就可以创建新段落

`Shift` + `Return` 创建单行中断。

### 标题

### 块引用

> 这里是块引用
> 感觉没有间隔的一行用`Shift` + `Return` 创建
>
> > 嵌套块引用

### 列表

- *
- -
- +

1. 第一项
2. 第二项

### 任务列表

- [ ] 一个任务列表-  [ ]


- [x] 已经完成的任务- [x]

### 代码

```gfm
Here's an example:

​```
function test() {
  console.log("notice the blank line before this function?");
}
​```

syntax highlighting:
​```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
​```
```

### 数学

使用**MathJax**渲染*LaTex*数学表达式

输入`$$` 后面跟上源码

$$\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\\end{vmatrix}$$

### 表格

| 我    | 反    | 正    |
| :--- | ---- | ---- |
| 不    | 会    | 怎    |
| 用    | 这    | 个    |
| 表    | 格    | 你    |
| 看    | 办    | 着    |

### 脚注

定义脚注

[^footnote]: Here is the *text* of the **footnote**.

然后就可以使用了

this example[^footnote]

### 水平线

***

---

### TOC

输入`[toc]` 可以显示内容表格

[TOC]

### 行内元素

Typora会将行内元素边变输入渲染

### 链接

Markdown有两种链接：行内链接和引用，两种都由方括号作为定界符

This is [an example](http://www.baidu.com/ "标题") 内部链接,鼠标悬停时应该显示标题

[This link](http://www.baidu.com/) 没有标题的链接

**你可以将href设置在头部**，这样可以创建一个书签让你跳转到所点击的部分。注意要按住Command

另一种风格的链接This is [an example][id] 引用风格链接

[id]: http://www.baidu.com

省略链接名

[google][]

然后定义

[google]: http://www.google.com

### URL

<>包围url，Typora可以自动转换不用括号

<gzzing@hotmail.com> gzzing@outlook.com

### Image

图片很像链接，但是前面要加！

![可选](http://cdn1.tnwcdn.com/wp-content/blogs.dir/1/files/2016/05/Tim-Cook-Neelie-Kroes-Startupfest-1592x796.jpg)

可以通过浏览器拖拽来插入图片。点击图片修改Markdown代码。拖拽时使用相对路径

如果你在使用Markdown来构建站点，为了能在本地访问，你需要在YAML Front Matters中指出url前缀，使用属性`typora-root-url:/User/Sameul/Website/typora.io/` 然后所有url都有这个前缀了

### 强调

*asterisk* _underscores_ 

**asterisk** __underscores__

### 删除线

~~删除线~~用两个~~

### 下划线

原生支持cmd + u

### Emoji

:smile:用两个：：包围:cry:

### 数学公式

$\lim_{x \to \infty}\exp(-x) = 0$

