![image](https://user-images.githubusercontent.com/73643473/104328236-fa3b9f00-552e-11eb-81f1-1a8204ca2e16.png)

```html
<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>나의 홈페이지</title>
	<style>
		#header{
		background-color: #7b98c7;
		width: 650px;
		height: 130px; 
		}
		div{
		margin-left: 28%;
		}
		
		#footer{
		background-color: #7b98c7;
		width: 650px;
		height: 100px;
		}
	
		#main{
		border: black soild 1px;
		width:650px;
		min-height: 380px;
		margin-left: 28%;
		}
		
		h1 {
		font-size: 60px;
		font-family: "한컴 쿨재즈 B";
		}
		
		ul{
		  list-style:none;
		  margin:0;
          padding:0;
          margin-left: 19%;
		}
		li {
    	margin: 0 0 0 0;
   		padding: 0 0 0 0;
  		border : 0;
 		float: left;
		}
		
		
		a:hover { text-decoration:none; color:#EDA900;}
	</style>
</head>
<body>
	<div align="center" id = "header">
		<h1>나의 홈페이지</h1>
		<nav>
		<ul>
			<li><a href="#">LOGIN</a><span>&nbsp;|&nbsp;</span></li>
			<li><a href="#">LOGOUT</a><span>&nbsp;|&nbsp;</span></li>
			<li><a href="#">JOIN</a><span>&nbsp;|&nbsp;</span></li>
			<li><a href="#">MY PAGE</a><span>&nbsp;|&nbsp;</span></li>
			<li><a href="#">BOARD</a><span>&nbsp;|&nbsp;</span></li>
			<li><a href="#">FILES</a></li>
		</ul>
		</nav>
	</div>
	
	<div id="main">
	<h1>이것은 본문</h1>
	</div>
	<!-- footer -->
	<div id="footer">
		<p align= "center"> &copy;2021. HyeonSeong Lee. All Rights Reserved.</p>
	</div>
</body>
</html>
```
