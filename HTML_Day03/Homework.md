```html
<!--로그인 페이지-->
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>로그인</title>
</head>
<style>
    #wrapper{
    width:50%;
    margin: 0 auto;
    }
    .login{
    width:300px;
    height:20px;
    }


</style>
<body marginheight="150;" background="C:\Users\PC!\Desktop\html\image\bg4.jpg">
<div id="wrapper">
    <table>
        <tr>
            <td>
                <fieldset style="width:300px; height:400px; padding: 20px; background-color: #0f68a3;">
                    <img src="C:\Users\PC!\Desktop\html\image\bg1.jpg" width="300px;" height="400px;">
                </fieldset>
            </td>

            <td>
                <form action="#" method="post">
                    <fieldset style="height:400px; padding: 20px; background-color:#0cc5eb; " >
                        <img src="C:\Users\PC!\Desktop\html\image\bg9.jpg" width="300" height="200;"/><br>

                        <label for="f_id">아이디(ID)</label><br>
                        <input name="id" class="login" type="text" id="f_id" placeholder="아이디를 입력하세요.(Type your ID)"
                               required><br><br>

                        <label style for="f_pw">비밀번호(Password)</label><br>
                        <input name="password" class="login" type="password" id="f_pw"
                               placeholder="비밀번호를 입력하세요. (Type your password)" required><br>
                        <br>
                        <table>
                            <tr>
                                <td style="width:40px;"></td>
                                <td><input type="submit" value="로그인"></td>
                                <td><a href="Homework_03(5~9).html"><input type="button" value="회원가입"></a></td>
                                <td><input type="button" value="ID/PW 찾기"><br></td>
                            </tr>
                        </table>
                        <table>
                            <tr>
                                <td style="width:80px;"></td>
                                <td><input type="checkbox"><label>Remember Me</label></td>
                            </tr>
                        </table>
                    </fieldset>
                </form>
            </td>
        </tr>
    </table>
</div>

</body>
</html>
```
![homework02_log](https://user-images.githubusercontent.com/73643473/103483017-b73f4480-4e27-11eb-8036-6fca14b99478.png)
