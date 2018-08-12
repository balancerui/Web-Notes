一：关于HTML学习笔记
HTML是超文本标记语言，它的作用就是在制作前端页面时展现的内容。
<!DOCTYPE HTMl>
<html>
<head>
<meta charset="UTF-8">
<title>邓瑞的学习笔记</title>
</head>
<body>
  <h1>我的HTMl</h1>
  <p>这是一个段落</p>
</body>
</html>
基本的形式就是以上这种，记得各种标签所代表的含义。

二：HTML的标签元素
<!--...-->		定义一行注释
<br>			定义换行
<abbr>			定义一个缩写
<p>				定义段落
<h1></h1>		定义标题
<b></b>			定义粗体
<i></i>			斜体文本
<sub></sub>		定义斜体
<form></form>	定义表单
<input></input>	定义输入控件
<div></div>		定义节
<button></button>	定义按钮
<link></link>		定义文档与外部资源的关系
<table></table>		定义表格
<th></th>	定义表格中的表头单元格
<tr></tr>	定义表格中的行
<td></td>	定义表格中数据
<select></select>	定义下拉选择框
<option></option>	定义下拉选择框中的选项
<password></password>	定义密码类型
<disable>	禁用
<readonly>	只读
<textarea> 	定义文本框
<radio>	定义单选按钮
<CheckBoxes>	定义复选框
<reset>	定义重置按钮
<del></del>		定义删除文本
<submit>		定义提交按钮
<alt>	图片无法显示时，将显示alt中的文本信息

三：HTML的规范
（1）定义需注意的地方
1.定义完段落<p>以后，可以用align来进行规范，设置段落。包括left，right，center。
2.定义超链接<a href="www.baidu.com">百度页面</a> 
3.定义图片<img src="/img/logo.png" weight="" high="">
4.实现缩写<abbr title="etcetera">etc.</abbr>
5.改变文字方向<p><bdo dir="rtl">该段落文字从右到左显示</bdo></p>
6.链接的target属性<a href="xx.com" target="_blank">打开该链接时，会跳转页面</a>
7.邮件发送时，需要使用关键字：mailto
	<a href="mailto:dengr@163.com?subject=邮件主题&body=邮件主体"></a>

（2）HTML<head>元素
head元素包含了所有的头部标签元素，在<head>元素中可以插入script、css、以及各种meta信息
以下是可以加入到<head>中的标签元素<title><script><css><meta><base><style><link>
<base>元素描述了基本的链接地址(默认链接)

（3）HTML<link>元素
定义了元素与外部的联系
<link rel="stylesheet" type="text/css" href="xxx.com" />

（4）HTMl<CSS>属性
用于渲染HTML的元素
<!DOCTYPE HTMl>
<html>
<head>
<meta charset="UTF-8">
<title>邓瑞的学习笔记</title>
<style>
	h1 {background:red}
	p {color:blue}
</style>
</head>
<body>
  <h1>我的HTMl</h1>
  <p>这是一个段落</p>
</body>
</html>

（5）如何使用CSS
①内联样式 ②内部样式表 ③外部引用
<p style="color:red;margin=left:20px;">这是一个段落</p>
<style>
	h1 {background:red}
	p {color:blue}
</style>
<link rel="stylesheet" type="text/css" href="xxx.css" />

（6）图片属性
<img src="图片位置" alt="显示文本" weight=“宽” height="高" align="">

（7）HTML表格
表格由<table>标签来定义。<tr>定义表格的行  <td>定义表格的数据	<th>对表格的表头进行定义
数据单元格中可以包括文本、图片、列表、段落、表单、水平线、表格等
<table border="1"	cellpadding="10">
	<tr>
		<td>数据</td>
	</tr>
</table>
<caption>定义表格的标题	<colspan>定义跨行 <rowspan>定义跨列
<cellpadding>定义表格的内容和边框之间的空白

（8）HTML列表
①有序列表<ol>	②无序列表<ul>	③自定义列表
自定义列表以<dl>标签开始，列表项以<dt>开始，自定义列表项的定义以<dd>开始
<dl>
<dt>coffee</dt>
	<dd>-black hot drink<dd>
<dt>Milk</dt>
	<dd>-black hot drink<dd>
</dl>

（9）HTML区块 <div>	<span>
块级元素在浏览器显示时，通常会以新行来开始和结束；如<h1><p><ul><table><div>
内联元素再浏览器显示时，不会以新行开始。<b><td><a><img><span>
<div>块级元素，用于组合其他HTML元素的容器
<span>用作文本的容器，与css一起使用时，可以为部分文本设置样式属性

（10）HTML表单和输入
First name:<input type="text" name="firstname"><br>

（11）HTML表单
表单元素是是允许用户在表单中输入内容，比如文本域、下拉框、单选框、复选框等标签元素
<form action="" >
	<input type="password" name="密码" value="male">male<br>
</form>
表单元素中的标签元素
①form表单 ②input输入 ③type类型 ④单选radio ⑤复选checkboxes ⑥submit提交 ⑦reset重置 ⑧select下拉框 
⑨option下拉框中的选项 ⑩textarea文本 （11）password密码 （12）button按钮 （13）disable禁用 
（14）readonly只读 （15）selected带有预选值的 （16）lable标签，一般为输入标签
（17）filedset定义一组相关的表单元素，并用外框包含起来 （18）legend定义filedset元素的标题
（19）value提交数据到服务器的值 （20）checked默认选中 
注意：同一组的单选按钮，name取值一定要一致

（12）HTML框架
使用框架，可以同一个浏览器窗口显示多个页面
<iframe src="URL"></iframe>
①去除边框
<iframe src="URL" frameborder="0"></iframe>
②显示目标链接页面
<iframe src="url" name="frame"></frame>
<a href="xxx.com" target="frame"></a>

（13）HTML脚本
JavaScript脚本使页面具有更强的动态和交互性。常用于图片操作、表单验证、内容动态更新。
<script>
	document.write("hello world");
</script>

javascript事件响应
document.getElementById("demo").InnerHtml="hello world";

（14）HTML速查列表
一个网页地址实例: http://www.runoob.com/html/html-tutorial.html 语法规则:
scheme://host.domain:port/path/filename
说明:
scheme - 定义因特网服务的类型。最常见的类型是 http
host - 定义域主机（http 的默认主机是 www）
domain - 定义因特网域名，比如 runoob.com
:port - 定义主机上的端口号（http 的默认端口号是 80）
path - 定义服务器上的路径（如果省略，则文档必须位于网站的根目录中）。
filename - 定义文档/资源的名称

常见的 URL Scheme
以下是一些URL scheme：
Scheme	访问	用于...
http	超文本传输协议	以 http:// 开头的普通网页。不加密。
https	安全超文本传输协议	安全网页，加密所有信息交换。
ftp	文件传输协议	用于将文件下载或上传至网站。
file	 	您计算机上的文件。

URL 字符编码
URL 只能使用 ASCII 字符集.
来通过因特网进行发送。由于 URL 常常会包含 ASCII 集合之外的字符，URL 必须转换为有效的 ASCII 格式。
URL 编码使用 "%" 其后跟随两位的十六进制数来替换非 ASCII 字符。
URL 不能包含空格。URL 编码通常使用 + 来替换空格。

