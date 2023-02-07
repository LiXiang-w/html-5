#  <span style="color:Magenta;font-size:100px;line-height:">   HTML文档结构</span>

红色代表大标题内容

Color:文字颜色
		background:背景颜色
		font-size:字体大小
		font-family:字体
		align = "center" 居中

Mediumorchid

Magenta

---



## <span style='color:red;font-size:80px'>HTML5规范解析</span>

```html
<!DOCTYPE html>
```

<u>!号：表申明的意思。这一行代码的意思是：下面的文档标签将以html5规范去解析</u>

```html
<html lang="en">	告诉html这是一个英文网站	lang:是language的缩写语言的意思
```



---



## <span style='color:red;font-size:80px'>自动生成快捷键标题</span>

```html
!加TAB自动生成
输入HTML:5+TAB自动生成
```

---



## <span style='color:red;font-size:80px'>网站对应设置</span>

### 1. meta元，用来完成对应设置

#### (1).字符集，编码设置

```html
在head里标签内，可以通过<meta>标签的charset属性来规定HTML文档应该使用那种字符编码
<meta charset="utf-8"> 
charset常用的值有：GB2312、BIG5、GBK和UTF-8，其中UTF-8也被称为万国码，基本包含了全世界所有国家需要用到的字符
```

#### (2).网站搜索关键字

```html
<meta name="keywords" content="">设置一个网站的搜索关键字
			keywords:关键字		content:搜索关键字内容写在这里面
```

#### (3).网站的描述内容

```html
 <meta name="description" content=""> 网站的描述内容
			description:描述		content:网站描述内容写在这里
```

### 2. 网站小图标

```html
	快捷方式（link:favicon）
<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
	shortcut icon:小图标				href:放置图标地址			type:图标类型
```

---



## Css样式

### 1.书写样式<span style='color:red;font-size:40px'></span>

```html
<style>书写样式放在这个地方</style>
```

###  2.如果引入外部样式文件

```html
快捷方式（link:css）
  <link rel="stylesheet"  href="style.css">
		stylesheet:样式表;类型	 href:样式文件写在这里面
```





## <span style='color:red;font-size:80px'>基本标签</span>



### <span style='color:Magenta;font-size:40px'>1. 标题标签h1-h6（重要）</span>

```html
HTML提供了6个等级的网页标题
即：<h1>-<h6>
  <h1>我是一级标签</h1>
  h为单词head的缩写，意为头部、标题
  标签语以：作为标题使用，并且依据重要性递减
  特点：
  		1.加了标题的文字会变的加粗，字号也会依次变大
  		2.一个标题独占一行
```



### <span style='color:Magenta;font-size:40px'>2. 段落标签p（重要）</span>

```html
									双标签
在网页中，要把文字有条理地显示出来，就需要将这些文字分段显示。在HTML标签中，<p>标签用于定义段落，它可以将整个网页分为若干个段落。
<p>我是一个段落标签</p>		
	p是单词 paragraph的缩写，意为段落。
标签语义：可以把HTML文档分割为若干段落
特点：
		1.文本在一个段落中会根据游览器窗口的大小自动换行。
		2.段落和段落之间保有空隙。
```



### <span style="color:Magenta;font-size:40px">3. br换行标签（重要 ）</span>

```html
						单标签
在HTML中，一个段落中的文字会从左到右依次排列，直到游览器窗口的右端，然后才自动换行。如果希望某段文字强制换行显示，就需要使用换行标签<br />
	<br />
单词break的缩写，意为打断、换行。
标签语义：强制换行。
特点：
		1.<br />是个单标签。
		2.<br />标签只是简单地开始新的一行，跟段落不一样，段落之间会插入一些垂直的距离
```

---



### <span style="color:Magenta;font-size:40px">4. 文本格式化标签</span>

```html
在网页中，有时候需要为文字设置粗体、斜体、或下划线效果,这时候就需要用到HTML中的文本格式化标签，使用文字以特殊的方式显示。
标签语义：突出重要性，比普通文字更重要
	加粗：<strong></strong>或者<b></b> 说明：更推荐使		用<strong>标签加粗 语义更强烈
    倾斜：<em></em>或者<i></i> 说明：更推荐使用<em>标签加粗 语义更强烈
    删除线<del></del>或者<s></s> 说明：更推荐使用<del>标签加粗 语义更强烈
    下划线<ins></ins>或者<u></u>说明：更推荐使用<ins>标签加粗 语义更强烈
```



---





### <span style="color:Magenta;font-size:40px">5.div和span布局标签</span>

```html
<div>和<span>是没有语义的，它们就是一个盒子，用来装内容的
  <div>这是div</div>
  <span>这是span</span>
  div是division的缩写，表示分割、分区
  span意为跨度、跨距
  特点：
  		1. <div>标签用来布局，但是现在一行只能放一<div>。大盒子 
  		2.<span>标签用来布局，一行上可以多个<span>.小盒子 
```

---



### <span style="color:Magenta;font-size:40px">6.图像标签和路径（重点）</span>

#### <span style="color:Mediumorchid;font-size:30px">1. img图像标签</span>

```html
1. 图像标签
在HTML标签中，<img>标签用于定义HTML页面中的图像。
<img src="图像URL" /> 	单词image的缩写，意为图像。
		 src是<img>标签的必须属性，它用于指定图像文件的路径和文件名。
所谓属性：简单理解就是属于这个图像标签的特性。
```

```c
/*
图像标签属性注意点：
1.图像标签可以拥有多个属性，必须写字标签名后面
2.属性之间不分先后顺序，标签名与属性、属性与属性之间均以空格分开。
3.属性采取键值对的格式，即key= "value"的格式，属性="属性值"。
			*/
```



| 属性   | 属性值   | 说明                                 |
| :----- | :------- | :----------------------------------- |
| src    | 图片路径 | 必须属性                             |
| alt    | 文本     | 替换文本。图像不能显示的文字         |
| title  | 文本     | 提示文本。鼠标放到图像上，显示的文字 |
| width  | 像素     | 设置图像的宽度                       |
| height | 像素     | 设置图像的高度                       |
| border | 像素     | 设置图像的边框粗细                   |

#### <span style="color:Mediumorchid;font-size:30px">2.路径：</span>

页面中的图片会非常多，通常我们会新建一个文件夹来存放这些图像文件(images)，这时再查找图像，就需要采用“路径”的方式来指定图像文件的位置。
路径可以分为：

相对路径：以饮用文件所在位置为参考基础，而建立出的目录路径，简单来说，图片相当于HTML 的页面的位置

绝对路径：是指目录下的绝对位置，直接到达目标位置，通常是从盘符开始的路径。
	例如：“D\web\img\logo.gif”或完整的网络地址：“http://www.itcast.cn/images/logo.gif”。

| 相对路径分裂 | 符号 | 说明                                                        |
| ------------ | ---- | ----------------------------------------------------------- |
| 同一级路径   |      | 图像文件位于HTML文件同一级 如\<img src="baidu.gif /">       |
| 下一级路径   | /    | 图像文件位于HTML文件下一级 如\<img src="images/baidu.gif/"> |
| 上一级路径   | ../  | 图像文件位于HTML文件上一级 如\<img src="../baidu.gif/">     |



---



### <span style="color:Magenta;font-size:40px">7.超链接标签（重点）</span>

##### <span style="color:Mediumorchid;font-size:30px">1.链接的语法格式</span>

```html
在HTML标签中，<a>标签用于定义超链接，作用是从一个页面链接到另一页面.
  1.超链接到语法格式：
  				<a href="跳转目标" target="目标窗口的弹出方式">文本或图像</a>
  a是单词anchor的缩写，意为：锚
  <!--两个属性的作用如下：
  	href：用于指定链接目标的url地址，（必须属性）当为标签应用href属性时，它就具有了超链接的功能
  	target：用于指定链接页面的打开方式，其中_self为默认值,_blank为新窗口中打开方式。-->
```

##### <span style="color:Mediumorchid;font-size:30px">2.链接分类</span>

```html
1. 外部链接，例如<a href="http://www.baidu.com">白度</a>
2. 内部链接：网站内部页面之间的相互链接。直接链接内部页面名称即 可，例如<a href="index.html">首页</a>
3.空链接：如果当时没有确定链接目标时，<a href="#">首页</a>
4. 下载链接：如果href里面地址是一个文件或者压缩包，会下载这个文件
5. 网页元素链接：在网页中的各种网页元素，如文本、图像、表格、音频、视频等都可以添加超链接
```

<span style="color:red">锚点定位链接</span>

```html
6. <!--锚点链接：点我们点击链接，可以快速定位到页面中的某个位置。-->
<-- 1.在链接文本的href属性中，设置属性值为#名字的形式，如<a href="#two">第二集</a>   -->
<-- 找到目标位置标签，里面添加一个id属性 = 刚才的名字，如<h3 id="two">第二集介绍</h3> -->
```



---



### <span style="color:Magenta;font-size:40px">8.HTML中的注释和特殊字符</span>

#### <span style="color:Mediumorchid;font-size:30px">1. 注释</span>

```html
如果需要在HTML文档中添加一些便于阅读和理解但又不需要显示在页面中的注释文字，就需要使用注释标签
< -- HTML中的注释以“<!--开头，以“-->”结束
<!--注释语句-->
< 快捷键:ctrl + /	>

```

#### <span style="color:Mediumorchid;font-size:30px">2.特殊字符</span>

```html
在HTML页面中，一些特俗的符号很难或者不方便直接使用，此时我们就可以使用下面的字符来替代
```



| 特殊字符 | 描述     | 字符的代码(后面全加分号;) |
| -------- | -------- | ------------------------- |
|          | 空格符   | &nbsp                     |
| <        | 小于号   | &lt                       |
| >        | 大于号   | &gt                       |
| &        | 和号     | &amp                      |
| ¥        | 人民币   | &yen                      |
| ©️        | 版权     | &copy                     |
| ®️        | 注册商标 | &reg                      |
| ℃        | 摄氏度   | &deg                      |
| ±        | 正负号   | &plusmn                   |

| ✖️    | 乘号 | &times  |
| ---- | ---- | ------- |
| ➗    | 除号 | &divide |

**空格大于号小于号经常用**

---

 

```html
单标签
<hr />生成一条水平线，主要用来装修用
```

---



### 6.a标签超文本跳转

==<a></a>实现链接跳转==
	   a标签有href，target属性

```html
<a href="URL或者页面文档" title=“提示文字” target="_blank">text</a>
```

1. href：内可以输入网址。后面加上标题
   2. title：代表鼠标指向后面标题出单提示文字

```c
	 target属性有4个值：
			<a href="URL" target="_blank">text</a>
			_blank:游览器总在一个新打开的、未命名的窗口载入目标文档
		<a href="URL" target="_self">text</a>
		_self:默认当前窗口

		_parent:

		_top:
href：内可以输入网址。后面加上标题
	title：代表鼠标指向后面标题出单提示文字
```

---



### 7.img图片标签

```html
单标签
<img src="URL" title="鼠标放置提示文字" alt="提示文字">
img:用来加载外部图片图像
src:用来设定加载的图片或图像的路径
title：代表鼠标指向后面标题出单提示文字
alt:当这个图片显示不成功时，显示的内容
```

### 8.span标签

```html
<span></span>和div标签作用一样都是用来布局的，不同的是div会单独在一行，而span不会,用于行内布局
<span>span1</span>
<span>span2</span>
	不会和div一样自动独自一行，会挨着
```

### 9.ul/oi列表

```html
<ul></ul>是无序列表
<ol></ol>是有序列表
它们的列表内容都用的li标签
<ul>
```

## 基本属性

### 1.width长度

```html
<width=“1%”>说明长度为百分之1
```

### 2.height高度

```html
<height="1px">说明高度为1像素
```

