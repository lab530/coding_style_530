<h1 style="text-align:center">530 Markdown 排版规则</h1>

## 目录

- [目录](#目录)
- [基本记号](#基本记号)
- [文本](#文本)
- [标题](#标题)
- [加重记号](#加重记号)
- [列表](#列表)
- [其他](#其他)

## 基本记号

``` markdown
标题记号：
# H1 到
###### H6 号标题

加重记号：
*Italic*
**Bold**
***Bold Italic***

非计数列表记号，统一使用短线：
- AAA
- BBB
- CCC

计数列表记号：
1. AAA
2. BBB
3. CCC

分割线，统一使用三个短线：
---

行内代码、代码块：
C 语言类型 `int`, `short`, `long`, `long long`
''' c++
int main() { cout << "hello"; }
'''  无法在此处使用反引号，这里使用单引号代替，后同

MathJax 行内公式、公式：
对于 $\forall a, b \in \mathbb{R} \cup b \not ={0}$，有
$$
\frac{a}{b} \in \mathbb{R}
$$

超链接、图片：
[《中文文案排版指北》](https://mazhuang.org/wiki/chinese-copywriting-guidelines/)
![Baidu](https://www.baidu.com/img/PCtm_d9c8750bed0b3c7d089fa7d55720d6cf.png)
```

除以上出现的符号以外，其他符号请勿使用，以免造成格式混乱。

## 文本

具体参考[《中文文案排版指北》](https://mazhuang.org/wiki/chinese-copywriting-guidelines/)。

需要强调的是：

- 字母、数字与汉字之间一定需要有空格相隔。具体参考排版指北；
- 不使用「、」代替“、”；
- 标点符号使用需正确。句末一定要加上句号。列表的项结尾使用分号，最后一项使用句号结尾。
- 不同元素（element）之间使用**一个**空行隔开，这里的元素指的是 HTML 元素。参考：

  ``` markdown
  ## 标题

  正文第一段

  正文第二段第一行（注意这后面需要有至少两个以上的空格才会产生自然换行）  
  第二行

  1. 列表
  2. 列表
  3. 列表

  代码：

  ''' c++
  int apples;
  '''
  ```

  且不要使用多个连续空行。
- 不考虑使用除了本文提到的任何 HTML 标签，以免排版错乱。
- 嵌套元素使用 Tab 对齐。

## 标题

除了使用井号的 H1~H6，可使用 HTML 标签对标题进行居中处理：

``` html
<h1 style="text-align:center">530 Markdown 排版规则</h1>
```

请不要出现其他自定义格式扰乱排版。

## 加重记号

使用 Italic 字体代替删除线使用。

尽可能使用 Bold 字体标记非常重点的内容。

尽可能不要使用 Bold Italic 字体。

## 列表

列表部分格式参考[文本](#文本)。

如果在列表前有明确数量的内容指示，使用计数列表。如：

``` markdown
要注意以下三点：

1. AAA
2. BBB
3. CCC
```

其余情况请使用无计数列表。

## 其他

其他无特殊要求的，一律尽量保证简洁、不冗余。
