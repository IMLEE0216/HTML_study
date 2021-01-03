```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Homework</title>
</head>
    <style>
    h1{
    color: #dddddd;
    }

    h2{
    color: #21db53;
    }

    h3{
    color: #bd6609;
    }

    table{
        border: black solid 2px;
        min-with: 100%;
        min-height: 100%;
        border-collapse: collapse;
    }

    td{
     border: black solid 2px;
    }

    th{
    border: black solid 2px;
    color: tomato;
    font-size: 20px;
    }

    .red :hover{
    color: tomato;
    }

    .blue :hover{
    color: blue;
    }

    span{
    border: tomato 1px solid;
    }

    div{
    border: blue 2px solid;
    }

    p{
    color: tomato;
    }
    </style>


<body>
    <h1>HTML 배우기</h1>
    <h2>HTML 배우기</h2>
    <h3>HTML 배우기</h3>
    <h4>HTML 배우기</h4>
    <h5><mark>HTML 배우기</mark></h5>
    <h6>HTML 배우기</h6>

    <p>뭘 이런걸 다~~</p>
    <table>
    <tr>
        <th colspan="8">일주일 식단표</th>
    </tr>

    <tr>
        <td>
        </td>
        <td align=center><p>일</p></td>
        <td align=center>월</td>
        <td align=center>화</td>
        <td align=center bgcolor="green">수</td>
        <td align=center bgcolor="yellow">목</td>
        <td align=center bgcolor="red">금</td>
        <td align=center><p>토</p></td>
    </tr>
    <tr>
        <td>아침</td>
        <td rowspan="3">
            <div>휴일</div>
        </td>
        <td>
            <ul class="red">
                <li>고구마</li>
                <li>흰우유</li>
                <li>삶은계란</li>
                <li><mark>바나나</mark></li>
            </ul>
        </td>
        <td>
            <ul class="blue">
                <li>감자</li>
                <li><mark>스프</mark></li>
                <li>빵</li>
                <li>딸기잼</li>
            </ul>
        </td>
        <td colspan="3" rowspan="3">
            <a href="https://www.naver.com"><img src="https://picsum.photos/id/870/200/300?grayscale&blur=2" style="border-radius: 15px"></a>
        </td>
        <td rowspan="3"> <div>휴일</div></td>

    </tr>
    <tr>
        <td>점심</td>
        <td>
            <ul class="red">
                <li>흰쌀밥</li>
                <li>소고기무국</li>
                <li>배추김치</li>
                <li><span>과일샐러드</span></li>
                <li>멸치볶음</li>
                <li>참외</li>
            </ul>
        </td>
        <td>
            <ul class="blue">
                <li>콩밥</li>
                <li>김치찌개</li>
                <li>열무김치</li>
                <li><del>야채햄볶음</del></li>
                <li>단호박샐러드</li>
                <li><span>딸기</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>저녁</td>
        <td colspan="2" align=center>집에서 먹어</td>
    </tr>
        <tr>
            <td colspan="8" align=center>수,목,금 - 방문</td>
        </tr>

    </table>
</body>
</html>
```
![homework](https://user-images.githubusercontent.com/73643473/103358480-053b0c00-4af9-11eb-8924-858480710567.png)
