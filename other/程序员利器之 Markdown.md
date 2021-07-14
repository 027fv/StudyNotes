> [程序员利器之 Markdown](//zhuanlan.zhihu.com/p/47475300)
> --------------------------------------------------

[<img src="https://pic1.zhimg.com/v2-e75b5383a665819f29220b1df311998e_s.jpg?source=2231c908" style="zoom:10%;" />](//www.zhihu.com/org/ling-kou-leetcode)[力扣（LeetCode）](//www.zhihu.com/org/ling-kou-leetcode)

[​](https://www.zhihu.com/question/48510028)

![](https://pic1.zhimg.com/v2-d9a999f0c7e37c0e5245e3221cc489f1_r.jpg?source=172ae18b)

⬇️ 基础小抄，请快速下滑 ⬇️  

> 程序员的工作效率往往高于平均值，究其原因，程序员的「懒惰」帮了大忙，哪怕是简单的重复性工作，他们也要用程序实践。「程序员的利器」系列文章巡礼那些能提高开发/工作效率的工具，帮你在职场/生活中节约时间。

Markdown 是一种轻量级的标记语言，它可以帮助你快速写作。在日常生活中，事项，清单，收发邮件，简历，公众号图文、工作文稿的撰写都可以使用 Markdown 来完成。相比于微软提供的 Word，Markdown 使用起来要简单快捷得多，非常「极简主义」和「极客精神」。当然，对于过于复杂的写作要求（比如写作时涉及到复杂的图文混排），选择 LaTeX 或者 Microsoft Word 更加合适。

Markdown 文本可以很容易的被转换为 HTML，PDF 之类的格式，方便在不同场合应用。

* * *

**支持 Markdown 的平台有哪些？**
-----------------------

几乎任何程序员使用的文本/代码编辑器，如 Atom，Sublime Text，Visual Studio Code，都支持 Markdown 文本的高亮显示，代码自动补全和实时渲染。对程序员非常友好。Markdown 的文件后缀名是 .md，在命名的时候需要注意。

![](https://pic3.zhimg.com/v2-64e03ddb80d93bda2a1044b431e9ed92_b.jpg)

当然如果出于某种原因你并不是用类似的代码编辑器，或者不太常编辑 Markdown 文本，也有一些在线的编辑工具可供使用，比如 [Dillinger](https://link.zhihu.com/?target=https%3A//dillinger.io/)，打开网页就可写作，同时支持实时预览。

如果你像我一样，有较为频繁的 Markdown 写作需求，同时希望写作环境尽可能简洁清新，可以把全部注意力集中在文字处理上。或者你不太使用代码编辑器，但仍想使用 Markdown 写作，我非常推荐你使用 Typora。

![](https://pic3.zhimg.com/v2-d48d328857a7024772b4b7db1bcc15b2_b.jpg)

这个软件的界面能让洁癖患者感到非常舒服，支持实时渲染模式和源代码模式，能快速导出为想要的文件格式并支持 laTeX 的数学公式语法。

Typora 预览

在其 [官方网站](https://link.zhihu.com/?target=https%3A//typora.io/) 上能下载不同的主题，为同一个 Markdown 文件提供不同的渲染效果。在中文写作时非常颜控的我经常使用「Han」这个主题。下图是该主题主页的一个范例。你也可以写用户 CSS 深度定制主题。

![](https://pic3.zhimg.com/v2-f20067bec5f4d3a4a89bbbb139b22132_b.jpg)

对于演讲或展示，诸如 [Remark](https://link.zhihu.com/?target=https%3A//remarkjs.com/%231) 和 [Cleaver](https://link.zhihu.com/?target=http%3A//jdan.github.io/cleaver/) 之类的工具都支持 Markdown 语法，帮助你用最短时间制作出在任何设备上都可以兼容（只要这个设备有浏览器）的展示页面。

对于邮件或新媒体写作，使用浏览器插件 [Markdown Here](https://link.zhihu.com/?target=https%3A//markdown-here.com/) 能最大程度帮你节省时间。简单来说，开启这个插件，在富文本编辑器（比如 Email 的编辑器，微信公众平台的编辑器）内输入 Markdown 文本，最后使用插件渲染页面，所有的 Markdown 都会被转化成 HTML 样式渲染在页面上。可以说是新媒体编辑和邮件发布者的利器。同时这个插件还支持深度定制 CSS。

* * *

**Markdown 基础**
---------------

Markdown 语法主要分为如下几大部分：标题，段落，引用，代码区块，强调，列表，分割线，链接，图片。

标题用 `#` 来标记，根据 `#` 的数量分为不同等级的标题。

```text
# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题
```

段落的前后要有空行，否则会被合并到一行显示。

使用 `>` 来表示一段引用，原本是用于在文章中引用别人的文章，现在经常被用于自动生成文章前言的样式。

```text
> 这是一段引用文字
```

强调使用两个 `*` 设置，斜体使用 `_` 来设置

```text
这是一段普通文本，**这是一段需要被强调的文本**，_这是一段斜体文本_
```

在行内插入代码时可以使用「\`」这个符号包裹代码，如果需要显示大段代码，使用三个相同的符号完成。

```text
​```javascrpit
	let msg = {language: 'JavaScript'};
	console.info(`这是一段 ${msg.language} 代码`);
​```

​```Python
	def msg = '这是一段 Python 代码'
	print(msg)
​```
```

使用数字与点和空格来声明有序列表，使用 `-` 声明无序列表。

```text
- 这是无序列表的第一项
- 这是无序列表的第二项

1. 这是有序列表的第一项
2. 这是有序列表的第二项
```

使用就是三个或以上 `*`，`-` 或 `_` 表示分割线。

```text
---
***
___

以上三种都可以被渲染成分割线
```

快速添加链接的方式是 `[]()`。

```text
[LeetCode](https://leetcode-cn.com/)
```

使用 `![]()` 的语法添加图片。

```text
![LeetCode T恤衫](https://leetcode-cn.com/static/images/store/tshirt_promo_cn.png)
```

除此之外，一些的 Markdown 编辑器还支持插入表格，公式，流程图等扩展语法。

* * *

**Reference**
-------------

1.  [https://zh.wikipedia.org/zh-hans/Markdown](https://link.zhihu.com/?target=https%3A//zh.wikipedia.org/zh-hans/Markdown)
2.  [https://www.markdownguide.org/getting-started](https://link.zhihu.com/?target=https%3A//www.markdownguide.org/getting-started)

  

作者：宫业奇

[编辑于 2018-11-04](//zhuanlan.zhihu.com/p/47475300)

赞同 295​

10 条评论

分享

取消收藏​ 举报收起​