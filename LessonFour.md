# HTML
## 什么是HTML
超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。
您可以使用 HTML 来建立自己的 WEB 站点，HTML 运行在浏览器上，由浏览器来解析。

## html基本构成
	<!DOCTYPE html>
	<html>
	<head>
	<title></title>
	</head>
	<body>
	</body>
	<footer>
	</footer>
	</html>

### 比如百度：https://www.baidu.com/<br/>

## 常用的html控件：
### div
   举例`<div></div>`

### table
   举例

### 引入
   举例

### 下拉框
   举例

### 单选框(radio)
   举例

### 多选框(checkbox)
   举例

### 表单和输入(form,input)
   举例

### 注释
   举例

### 标签一览
https://www.runoob.com/tags/html-reference.html

***
***
***
***
***


# CSS
## 什么是CSS
是在 HTML 4 开始使用的,是为了更好的渲染HTML元素而引入的.

## Css如何使用

### 内联样式- 在HTML元素中使用"style" 属性
	<div style="XXXXX">


### 内部样式表 -在HTML文档头部 `<head>` 区域使用`<style>` 元素 来包含CSS
	<style src="XXXX">
	<header>

### 外部引用 - 使用外部 CSS 文件
	<link rel="stylesheet" href="标签路径">

***
***
***
***
***

# JS
## 什么是JS
JS（JavaScript） 是 即时编译型的语言。主要应用于web端
所有现代的 HTML 页面都可以使用 JavaScript。

### 书写位置
	<script>
	</script>

## 引入方法
### 内联样式- 在HTML元素中使用"script" 属性
### 引入js文件
	<script src="script.js"></script>


## 常用JS
### 用法
   举例

### 调试
   举例

### 注释
   举例

### 变量
   举例

### 函数
   举例

### 字符串
   举例

### 运算符
   举例

### if
   举例

### for
   举例

### break
   举例

### 事件
   举例

### AJAX
	function ajaxTest(){
	var xhr;
	if(window.XMLHttpRequest){
	    xhr = new XMLHttpRequest();
	}else{
	    xhr = new ActiveXObject("Microsoft.XMLHTTP");
	}

	xhr.onreadystatechange = function() {
	  if (xhr.readyState === 4 && xhr.status === 200) {
	    var response = xhr.responseText;
	    // 在这里处理响应
	    console.log(response);
	  }
	};



xhr.open("GET", "https://www.runoob.com/try/ajax/ajax_info.txt", true);
xhr.send();

}



## 推荐学习网站：
https://www.runoob.com/<br/>
<span style="color:#333333"><img src="http://static.runoob.com/images/runoob-logo.png" width="50%"></span>

bilibili<br/>
https://www.bilibili.com/

