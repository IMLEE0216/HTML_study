### 회원가입

      회원가입 <form>을 하나 만들고
	    action : /ch02_servlet/Test03
	    method : post
	
	    아이디-<input>text
	    비밀번호 2번-<input>password, 
	    이메일-<input> text + <select> naver.com/nate.com/gmail.com/ 
	    운영진에게 한마디-<textarea>
	    등 등...
	 
	    Test03 서블릿
	    인자로 들어온 파라미터를 모두 받아 sysout 으로 출력
	    두 비밀번호가 같으면 "회원 가입 완료!"
	    다르면 "비밀번호가 일치하지 않습니다."

  
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>
<body>
	<form action="/ch02_servlet/Test03" method="post">
		<div>
			<label>아이디</label>
			<input name="ID" type="text" value="" placeholder="새로운 아이디를 입력하세요." required><br/>
			<hr/>
			
			<label>비밀번호</label>
			<input name="ne_password" type="password" value="" placeholder="새로운 비밀번호를 입력하세요." required><br/>
			<hr/>
			
			<label>비밀번호 확인</label>
			<input name="re_password" type="password" value="" placeholder="비밀번호를 다시 입력하세요." required><br/>
			<hr/>
			
			<label>이메일</label>
			<input name="email_id" type="text" value="" required>
			<label>@</label>
			<select name="email" required>
			<option>-------</option>
			<option value="naver">naver.com</option>
			<option value="gmail">gmail.com</option>
			<option value="nate">nate.com</option>
			<option value="hanmail">hanmail.net</option>
			</select><br/>			
			<hr/>
			
			<label></label>
			
			<input type="submit" name="signup" value="회원가입">
		</div>
	</form>
</body>
</html>
```

```java
package com.megait;

import java.io.IOException;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
@WebServlet("/Test03")
public class Test03 extends HttpServlet{

	@Override
	protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
		req.setCharacterEncoding("UTF-8");
	
		String id = req.getParameter("ID");
		String password = req.getParameter("ne_password");
		String re_password = req.getParameter("re_password");
		String email = req.getParameter("email_id");
		String emailad = req.getParameter("email");
		
		if(password.equals(re_password)) {
			String html = "<script>alert('Signup Success!!!!!');</script>";
			resp.getWriter().write(html);
			
			System.out.println("아이디 :" + id);
			System.out.println("비밀번호 :" + password);
			System.out.println("이메일 :" + email + "@" + emailad);
		} else {
			String html = "<script>alert('Signup failed@@@@@');</script>";
			resp.getWriter().write(html);
			
		}
	}
}
```

### 설문조사

      [quiz01-form.html]
      설문조사 페이지 만들기
      1. 혈액형 선택받기(Radio 사용)
        	O / A / AB / B / 기타 
      2. 통신사 선택받기(Radio 사용)
      	LG UPLUS / KT / SK / 기타
      3. 희망 과목 선택받기 (checkbox 사용) - 중복 선택 가능
         C++ / Python / Java / 기타
      4. submit (action="Quiz01" method="post")
      	<input type="submit" name="result" value="아주 좋음">
        <input type="submit" name="result" value="좋음">
        <input type="submit" name="result" value="보통">
        <input type="submit" name="result" value="별로">
        <input type="submit" name="result" value="아주 별로">
    
      [Quiz01 서블릿]
      받은 파라미터를 sysout으로 출력
      result 의 값을 화면으로 출력

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>

<body>
<form action="/ch02_servlet/Quiz01" method="post">

<label>형액형을 선택하세요.</label><br/>
<input type="radio" name="blood" value="A"> A형
<input type="radio" name="blood" value="B"> B형
<input type="radio" name="blood" value="AB"> AB형
<input type="radio" name="blood" value="O"> O형
<input type="radio" name="blood" value="기타"> 기타
<hr/>

<label>통신사를 선택하세요.</label><br/>
<input type="radio" name="mobile network" value="LG UPLUS"> LG UPLUS
<input type="radio" name="mobile network" value="KT"> KT
<input type="radio" name="mobile network" value="SKT"> SKT
<input type="radio" name="mobile network" value="알뜰"> 알뜰폰
<input type="radio" name="mobile network" value="기타"> 기타
<hr/>

<label>희망과목을 선택하세요.(중복 선택 가능)</label><br>
<input type="checkbox" name="sub" value="C++"> C++
<input type="checkbox" name="sub" value="Java"> Java
<input type="checkbox" name="sub" value="C++"> Python
<input type="checkbox" name="sub" value="Ruby"> Ruby
<input type="checkbox" name="sub" value="R"> R
<input type="checkbox" name="sub" value="Kotlin"> Kotlin
<input type="checkbox" name="sub" value="기타"> 기타
<hr/>

<label>설문조사 만족도</label><br>
	<input type="submit" name="result" value="아주 좋음">
    <input type="submit" name="result" value="좋음">
    <input type="submit" name="result" value="보통">
    <input type="submit" name="result" value="별로">
    <input type="submit" name="result" value="아주 별로">
</form>
</body>
</html>
```

```java
package com.megait;

import java.io.IOException;
import java.util.Arrays;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
@WebServlet("/Quiz01")
public class Quiz01 extends HttpServlet{

	@Override
	protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
		req.setCharacterEncoding("UTF-8");
		
		String[] bArr = req.getParameterValues("blood");
		String[] mArr = req.getParameterValues("mobile network");
		String[] sArr = req.getParameterValues("sub");
		String[] rArr = req.getParameterValues("result");
		
		System.out.println(Arrays.toString(bArr));
		System.out.println(Arrays.toString(mArr));
		System.out.println(Arrays.toString(sArr));
		System.out.println(Arrays.toString(rArr));
	}
}
```

### 랜덤 구구단
      랜덤하게 구구단 1문제를 내고 값을 입력 받는 <form> 구현
      "정답!" 혹은 "땡!"을 alert() 하기
      (서블릿, jsp, html 아무거나 선택)

```jsp
<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"%>
    
    <% int n = (int)(Math.random()*9)+2;
		int r = (int)(Math.random()*9)+1;
		int ans = n*r;
		//boolean result = ("answer".equals(ans));
		//String message = result? "Correct!!":"Wrong@@";
	%>

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>
<body>
	<form action = "/ch02_servlet/Quiz02" method="post">
	<input type=text name="n" value="<%= n%>"><label>X</label>
	<input type=text name="r" value="<%= r%>"><label>=</label>
	<input type=text name="answer" value="">
	<input type="submit" value="제출">
	</form>
</body>
</html>
```

```java
package com.megait;

import java.io.IOException;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

@WebServlet("/Quiz02")
public class Quiz02 extends HttpServlet{

	@Override
	protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
		req.setCharacterEncoding("UTF-8");
		
		String typeans = req.getParameter("answer");
		String n = req.getParameter("n");
		String r = req.getParameter("r");
		int ans = Integer.parseInt(n)*Integer.parseInt(r);
		
		boolean result = false;
		if(typeans.equals(Integer.toString(ans))) {
			result = true;
		}
		
		String html = "<script>alert(" + 
				(result?"'Correct!'":"'WrongTT'") +
				");</script>";
	
	resp.getWriter().write(html);
	}
}

```
