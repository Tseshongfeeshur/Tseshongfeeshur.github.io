# [<img src="图标.png" alt="Logo" style="zoom:7%;" />](index.html) 璃黯的杂货铺

###### **[`首页`](index.html)**		[`文章`](文章.html)		[`分享`](分享.html)		[`更多`](更多.html)		[`留言`](留言.html)		[`时刻`](时刻.html)

---

# `文章`

# 【转载】 L^A^T~E~X 公式篇

L^A^T~E~X ，始于公式，忠于优雅…

很长一段时间，数学公式的编辑都是采用 MathType 解决的，但是直到我遇到了 L^A^T~E~X 的公式便一见倾心、久久不能释怀…

## 简介

相信很多做学术的科研狗应该都是听过 L^A^T~E~X 排版写出来的 Paper 是多么的好看，颜值高。其实 L^A^T~E~X 简单来说就是一种文字处理软件/计算机标记语言。本文作为入门教程，不去过多解释其家族 T~E~X 、 L^A^T~E~X 、 CT~E~X 等等之间的伦理关系。一方面，用过 Word 的人都知道，排版的时间有的时候比写一篇文章的时间还长。更有甚者会遇到一些无解的玄学问题；另一方面，对于很多顶级期刊、会议对于投稿论文格式明确要求是 L^A^T~E~X ，拒收 Word 格式

L^A^T~E~X ，作为广义上的计算机标记语言（比如 HTML ），它继承了计算机语言的光荣传统，通过一些简单的代码表达出精确的含义，具有不二义性。其文章排版的结果可以完全按照你的想法来，不仅解决了玄学问题，渲染出来的文章优美；同时，其还可以通过简单的语法写出优雅高贵的数学公式，目前 Markdown 也已经支持 L^A^T~E~X 语法的公式

## 数学模式

在 L^A^T~E~X 数学模式中，公式有两种形式——行内公式和行间公式。前者公式嵌入在行内，适用于简单短小的公式；后者居中独占一行，适用于比较长或重要的公式。公式中的空格均会被忽略，可以使用命令`\quad`或`\qquad`实现

**行内公式**

```text
$ f(x) = a+b $
```

===>>> $ f(x) = a+b $

**行间公式**

```text
$$ f(x) = a+b $$
```

===>>>

$$ f(x) = a+b $$

## 数学结构

## 简单运算

拉丁字母、阿拉伯数字和 `+` `-` `*` `/` `=` 运算符均可以直接输入获得，命令`\cdot`表示乘法的圆点，命令`\neq`表示不等号，命令`\equiv`表示恒等于，命令`\bmod`表示取模

```text
$$ x+2-3*4/6=4/y + x\cdot y $$
```

===>>>

$$ x+2-3*4/6=4/y + x\cdot y $$

```text
$$ 0 \neq 1 \quad x \equiv x \quad 1 = 9 \bmod 2 $$
```

===>>>

$$ 0 \neq 1 \quad x \equiv x \quad 1 = 9 \bmod 2 $$

## 上下标

语法`_`表示下标、`^`表示上标，但上下标内容不止一个字符时，需用大括号括起来。单引号`'`表示求导

```text
$$ a_{ij}^{2} + b^3_{2}=x^{t} + y' + x''_{12} $$
```

===>>>

$$ a_{ij}^{2} + b^3_{2}=x^{t} + y' + x''_{12} $$

## 根号、分式

命令：`\sqrt`表示平方根，`\sqrt[n]`表示 n 次方根，`\frac`表示分式

```text
$$\sqrt{x} + \sqrt{x^{2}+\sqrt{y}} = \sqrt[3]{k_{i}} - \frac{x}{m}$$
```

===>>>

$$\sqrt{x} + \sqrt{x^{2}+\sqrt{y}} = \sqrt[3]{k_{i}} - \frac{x}{m}$$

## 上下标记

命令：`\overline`, `\underline` 分别在表达式上、下方画出水平线

```text
$$\overline{x+y} \qquad \underline{a+b}$$
```

===>>>

$$\overline{x+y} \qquad \underline{a+b}$$

命令：`\overbrace`, `\underbrace` 分别在表达式上、下方给出一个水平的大括号

```text
$$\overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26}$$
```

===>>>

$$\overbrace{1+2+\cdots+n}^{n个} \qquad \underbrace{a+b+\cdots+z}_{26}$$

## 向量

命令：`\vec`表示向量，`\overrightarrow`表示箭头向右的向量，`\overleftarrow`表示箭头向左的向量

```text
$$\vec{a} + \overrightarrow{AB} + \overleftarrow{DE}$$
```

===>>>

$$\vec{a} + \overrightarrow{AB} + \overleftarrow{DE}$$

## 积分、极限、求和、乘积

命令：`\int`表示积分，`\lim`表示极限， `\sum`表示求和，`\prod`表示乘积，`^`、`_`表示上、下限

```text
$$  \lim_{x \to \infty} x^2_{22} - \int_{1}^{5}x\mathrm{d}x + \sum_{n=1}^{20} n^{2} = \prod_{j=1}^{3} y_{j}  + \lim_{x \to -2} \frac{x-2}{x} $$
```

===>>>

$$  \lim_{x \to \infty} x^2_{22} - \int_{1}^{5}x\mathrm{d}x + \sum_{n=1}^{20} n^{2} = \prod_{j=1}^{3} y_{j}  + \lim_{x \to -2} \frac{x-2}{x} $$

## 三圆点

命令：`\ldots`点位于基线上，`\cdots`点设置为居中，`\vdots`使其垂直，`\ddots`对角线排列

```text
$$ x_{1},x_{2},\ldots,x_{5}  \quad x_{1} + x_{2} + \cdots + x_{n} $$
```

===>>>

$$ x_{1},x_{2},\ldots,x_{5}  \quad x_{1} + x_{2} + \cdots + x_{n} $$

## 重音符号

常用命令如下：

```text
$ \hat{x} $
```

===>>> $ \hat{x} $

```text
$ \bar{x} $
```

===>>> $ \bar{x} $

```text
$ \tilde{x} $
```

===>>> $ \tilde{x} $

## 矩阵

其采用矩阵环境实现矩阵排列，常用的矩阵环境有`matrix`、`bmatrix`、`vmatrix`、`pmatrix`，其区别为在于外面的括号不同：

![img](https://pic1.zhimg.com/80/v2-684e48900e810dff360c23b4ffe99680_1440w.webp)

下列代码中，&用于分隔列，\用于分隔行

```text
$$\begin{bmatrix}
1 & 2 & \cdots \\
67 & 95 & \cdots \\
\vdots  & \vdots & \ddots \\
\end{bmatrix}$$
```

 ===>>>

$$\begin{bmatrix}
1 & 2 & \cdots \\
67 & 95 & \cdots \\
\vdots  & \vdots & \ddots \\
\end{bmatrix}$$

## 希腊字母

希腊字母无法直接通过美式键盘输入获得。在 L^A^T~E~X 中通过反斜杠`\`加上其字母读音实现，将读音首字母大写即可输入其大写形式，详见下表

```text
$$ \alpha^{2} + \beta = \Theta  $$
```

===>>>

$$ \alpha^{2} + \beta = \Theta  $$$$ \alpha^{2} + \beta = \Theta  $$



![img](https://pic1.zhimg.com/80/v2-da3e717cf670582fbfbdddee33073524_1440w.webp)



## 多行公式

## 公式组合

通过`cases`环境实现公式的组合，`&`分隔公式和条件，还可以通过`\limits`来让 x→0 位于 lim 的正下方而非默认在 lim 符号的右下方显示

```text
$$D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases}$$
```

===>>>

$$D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases}$$

## 拆分单个公式

通过`split`环境实现公式拆分

```text
$$\begin{split}
\cos 2x &= \cos^2x - \sin^2x \\
&=2\cos^2x-1
\end{split}$$
```

===>>>

$$\begin{split}
\cos 2x &= \cos^2x - \sin^2x \\
&=2\cos^2x-1
\end{split}$$



*欢迎关注我的公众号（**个人简介处有微信公众号名称**），一起去寻找文明的痕迹～*

----

原作者：[Aaron Zhu](https://www.zhihu.com/people/zhu-guang-hua-520)

编辑&排版整理：璃黯

转载自[知乎](https://zhuanlan.zhihu.com/p/110756681)

