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


```html
<!--회원가입 페이지-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>회원가입</title>
    <SCRIPT LANGUAGE="JavaScript">

    </script>
    <style>
#wrapper{
width:50%;
margin: 0 auto;
}
label{
font-size:20px;
font-family:'굵은안상수체';
color: black;
}
h1{
color: black;
}

input{
height:30px;
}






    </style>
</head>
<body> <!--background="C:\Users\PC!\Desktop\html\image\bg17.jpg" style="background-size:100% 120%;"/bgcolor="#d5e1e3"-->

<div id="wrapper">
    <table>
        <tr>
            <td colspan="2">
                <h1 align="center" style="font-family:'굵은안상수체';">회원가입</h1>
            </td>
        </tr>
        <tr>
            <td>
                <img src="C:\Users\PC!\Desktop\html\image\bg15.jpg" width="370px;" height="573px;">
            </td>
            <td>

                <form action="create new account" method="post">
                    <fieldset style="padding: 20px; background-color:##d2d5d9;">
                        <table style="background-color:#ffffff">
                            <tr>
                                <td>
                                    <label for="n_id">아이디</label><br>
                                    <input name="input_1" style="width:210px;" value="" type="text" id="n_id"
                                           placeholder="새로운 아이디를 입력하세요." required>
                                    <input type="button" name="input_2" value="중복체크"><br><br>

                                    <label for="n_pw">비밀번호</label><br>
                                    <input name="input_3" style="width:300px;" type="password" id="n_pw"
                                           value="" placeholder="새로운 비밀번호를 입력하세요." required><br><br>

                                    <label for="r_pw">비밀번호 재확인</label><br>
                                    <input name="input_4" value="" style="width:300px;" type="password" id="r_pw"
                                           placeholder="비밀번호를 다시 입력하세요."
                                           required><br><br>

                                    <label>비밀번호 힌트 &nbsp;&nbsp;&nbsp;</label>
                                    <select style="width:210px; height:30px" name="input_5">
                                        <option value="0" selected>비밀번호 힌트</option>
                                        <option value="1">학창시절 나의 별명은?</option>
                                        <option value="2">아버지 성함은?</option>
                                        <option value="3">어머니 성함은?</option>
                                        <option value="4">가족 관계는?</option>
                                    </select><br>
                                    <input style="width:300px;" name="input_6" value="" type="text" id="hint"
                                           placeholder="힌트를 입력하세요."><br><br>

                                    <table>
                                        <tr>
                                            <td><label>이름(성별)</label></td>
                                            <td>
                                                <input type="radio" name="input_7" value="male">
                                            </td>
                                            <td>
                                                <span style="font-size:20px">남</span>
                                            </td>
                                            <td>
                                                <input type="radio" name="input_7" value="female">
                                            </td>
                                            <td>
                                                <span style="font-size:20px">여</span>
                                            </td>
                                            <td colspan="2"><label>생년월일</label></td>
                                        </tr>
                                        <tr>
                                            <td colspan="6"><input name="input_8" value="" type="text"
                                                                   placeholder="이름을 입력하세요."
                                                                   required></td>
                                            <td colspan="2"><input name="input_9" value="" type="date" required></td>
                                        </tr>
                                    </table>

                                    <label>휴대전화</label><br>
                                    <select name="input_9" style="height:30px;" required>
                                        <option value="" selected>---선택---</option>
                                        <option value="SKT">SKT</option>
                                        <option value="LG">LG</option>
                                        <option value="KT">KT</option>
                                    </select>
                                    <input style="width:220px;" name="input_10" value="" type="text"
                                           placeholder="'-'는 빼고 입력해주세요. ex)01012341234"
                                           required><br><br>

                                    <table>
                                        <tr>
                                            <td style="width:60px;"></td>
                                            <td><input type="submit" name="input_11" value="회원가입"></td>
                                            <td><input type="reset" name="input_12" value="초기화"></td>
                                            <td><a href="Homework_02(5~9).html"><input type="button" name="input_13" value="취소"></a></td>
                                        </tr>

                                    </table>
                                </td>
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

![homework03_signup](https://user-images.githubusercontent.com/73643473/103483068-100edd00-4e28-11eb-9a3d-bb80dba68fc3.png)

```html
<!--내 정보 보기 페이지-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>내 정보 보기</title>
</head>
<style>
 #wrapper{
    width:50%;
    margin: 0 auto;
    }

.front{
background-color: #d6d4d2;
}
table{
border-collapse: collapse;
}
.line{
border: #e8e8e8 solid 2px;"
}

</style>
<body>
<div id="wrapper">
<table>
    <tr>
        <td colspan="2">
            <h1>회원정보</h1>
        </td>
    </tr>
    <tr class="line">
        <td class="front">사용자 이름</td>
        <td>
            <div>
                <p>이현성</p>
                <p style="color:#a8a6a5;">이름의 정보가 변경 되었다면 수정을 통해 변경하실 수 있습니다.</p>
                <p style="margin:10px;">
                    <button>수정</button>
                </p>
            </div>
        </td>
    </tr>
    <tr class="line">
        <td class="front">휴대전화</td>
        <td>
            <div>
                <p>
                    <select>
                        <option>SKT</option>
                    </select>
                010-0000-1234</p>
                <p style="color:#a8a6a5;">휴대전화의 정보가 변경 되었다면 수정을 통해 변경하실 수 있습니다.</p>
                <p style="margin:10px;">
                <button>수정</button>
                </p>
            </div>
        </td>
    </tr>
    <tr class="line">
        <td class="front">
            비밀번호 힌트 <br>및 변경
        </td>
        <td>
            <div>
            <p>가족관계는?</p>
                <p style="color:#a8a6a5;">힌트의 질문과 답을 변경하시고 싶으시면 힌트변경을 통해 변경하실 수 있습니다.</p>
                <p style="margin:10px;">
                <button>힌트변경</button>
                </p>
            </div>
        </td>
    </tr>
    <tr class="line">
        <td class="front">
           생년월일
        </td>
        <td>
            <div>
                <p>1993.03.16</p>
                <p style="margin:10px;">
                    <button>수정</button>
                </p>
            </div>
        </td>
    </tr>
</table>
</div>
<div style="width:150px; margin:0 auto;">
<table>
    <tr>
        <td>
            <p></p>
            <p style="width:152px;"><button>수정 저장</button>&nbsp;<button>회원 탈퇴</button></p>
            <p></p>
        </td>
    </tr>
</table>
</div>
</body>
</html>
```

![homework04_info](https://user-images.githubusercontent.com/73643473/103483099-56fcd280-4e28-11eb-8fa3-3c2f0d810e70.png)

```html
<!--게시판 목록 페이지 혹은 상품 목록 페이지-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>게시판 목록 페이지</title>
</head>
<style>
 #wrapper{
    width:40%;
    margin: 0 auto;
    }
table{
border-collapse: collapse;
}

</style>

<body>
<div id="wrapper">
    <table>
        <tr style="border: black solid 2px;">
            <td bgcolor="#d2d5d9" width="80"><p align="center">번호</p></td>
            <td bgcolor="#d2d5d9"><p align="center">제목</p></td>
            <td bgcolor="#d2d5d9" width="110"><p align="center">글쓴이</p></td>
            <td bgcolor="#d2d5d9" width="100"><p align="center">날짜</p></td>
            <td bgcolor="#d2d5d9" width="80"><p align="center">조회수</p></td>
        </tr>
        <tr style="border: #d2d5d9 solid 1px;">
            <td><p align="center">1</p></td>
            <td><p>HTML 게시판 만드는 방법 좀 알려주세요</p></td>
            <td><p align="center">IMLEE</p></td>
            <td><p align="center">210102</p></td>
            <td><p align="center">5</p></td>
        </tr>
        <tr style="border: #d2d5d9 solid 1px;">
            <td><p align="center">2</p></td>
            <td><p>HTML 게시판 만드는 방법 좀...</p></td>
            <td><p align="center">IMLEE</p></td>
            <td><p align="center">210102</p></td>
            <td><p align="center">5</p></td>
        </tr>
        <tr style="border: #d2d5d9 solid 1px;">
            <td><p align="center">3</p></td>
            <td><p>HTML 게시판 만드는 방법 좀...</p></td>
            <td><p align="center">IMLEE</p></td>
            <td><p align="center">210102</p></td>
            <td><p align="center">5</p></td>
        </tr>
        <tr style="border: #d2d5d9 solid 1px;">
            <td><p align="center">4</p></td>
            <td><p>HTML 게시판 만드는 방법 좀...</p></td>
            <td><p align="center">IMLEE</p></td>
            <td><p align="center">210102</p></td>
            <td><p align="center">5</p></td>
        </tr >
        <tr>
            <td colspan="5" style="border: black solid 2px;">

            </td>
        </tr>
        <tr>
            <td>

            </td>
        </tr>
    </table>
</div>
    <div style="width:150px; margin:0 auto;">
        <p></p>
        <p style="width:152px;">
            <button>이전</button><button>1</button><button>2</button><button>다음</button>
        </p>
    </div>
</body>
</html>
```
![homework05_board](https://user-images.githubusercontent.com/73643473/103483128-975c5080-4e28-11eb-8649-9b0b29f423df.png)

```html
<!--게시판 상세 보기 혹은 상품 상세 보기-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>상세보기</title>
</head>
<style>
 #wrapper{
    width:500px;
    margin: 0 auto;
    }
    table{
    border-collapse: collapse;
    }


</style>
<body>
<div id="wrapper">
    <table>
        <tr>
            <td rowspan="2" width="400px;">
                <h1>게시물 보기</h1>
            </td>
            <td>
                <p align="center">글번호:</p>
            </td>
            <td><p>?</p></td>
        </tr>
        <tr>
            <td><p align="center">조회수:</p></td>
            <td><p>?</p></td>
        </tr>
    </table>
    <table>
        <tr style="border: #d2d5d9 solid 2px;">
            <td>
                <p>작성자</p>
            </td>
            <td width="403px;">
                <p>IMLEE</p>
            </td>
        </tr>
        <tr  style="border: #d2d5d9 solid 2px;">
            <td>
                <p>작성시간</p>
            </td>
            <td width="403px;">
                <p>210102</p>
            </td>
        </tr>
        <tr  style="border: #d2d5d9 solid 2px;">
            <td>
                <p>제목</p>
            </td>
            <td width="403px;">
                <p>HTML 게시판 만드는 방법 좀...</p>
            </td>
        </tr>
        <tr  style="border: #d2d5d9 solid 2px;">
            <td colspan="2">
                <p>
                    피카츄<br>
                    라이츄<br>
                    파이리<br>
                    꼬부기<br>
                    버터플<br>
                    야도란<br>
                </p>
            </td>
        </tr>
    </table>
</div>
<div style="width:150px; margin:0 auto;">
    <table>
        <tr>
            <td>
                <p><button>확인</button>&nbsp;<button>수정</button>&nbsp;<button>삭제</button></p>
            </td>
        </tr>
    </table>
</div>
</body>
</html>
```
![homework06_board](https://user-images.githubusercontent.com/73643473/103483160-be1a8700-4e28-11eb-9944-3f5798a7eafb.png)
