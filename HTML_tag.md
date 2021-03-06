# HTML 주요 태그

### 1. 단락 : p태그

- 단락의 앞과 뒤에 <p></p>

### 2. 줄바꿈 : br 태그

- 문단 끝에 <br>

### 3. 이미지 : img 태그

```html
<img src="img.jpg" width="300" height="400" alt="사진" title="증명사진>
```

- alt는 사진이 깨졌을 때 보이는 문구

### 4. 표 만들기

```html
<html><body>
 <table border="1">
  <thead>
   <tr>
    <th>이름</th>    <th>성별</th>  <th>주소</th> <th>회비</th>
   </tr>
  </thead>
  <tbody>
   <tr>
    <td>홍혜림</td>  <td>여자</td>   <td>경주</td>  <td>1000</td>
   </tr>
   <tr>
    <td>현재웅</td>  <td>남자</td>   <td>서울</td>  <td>10000</td>
   </tr>
  </tbody>
 <tfoot>
  <tr>
   <td>합계</td>  <td></td>  <td></td>  <td>11000</td>
  </tr>
 </tfoot>
</table>
</body></html>
```
![Untitled (5)](https://user-images.githubusercontent.com/67935853/105051293-f7522880-5ab1-11eb-8d29-228210f6e5da.png)

- 표 병합하기

```html
<tbody>
<tr>
<td>홍혜림</td>  <td>여자</td>   <td rowspan="2">서울</td>  <td>1000</td>
</tr>
<tr>
<td>현재웅</td>  <td>남자</td>     <td>10000</td>
</tr>
</tbody>
<tfoot>
<tr>
<td colspan="3">합계</td>   <td>11000</td>
</tr>
</tfoot>
```
![Untitled (6)](https://user-images.githubusercontent.com/67935853/105051356-046f1780-5ab2-11eb-98a3-2be4eac7379a.png)

### 5. form

- 기본

```html
<html>
<body>
<form action="[http://localhost/login.php](http://localhost/login.php)">
<p>아이디 : <input type="text" name ="id"></p>
<p>비밀번호 : <input type="password" name="pwd"></p>
<p>주소 : <input type="text" name="address"></p>
<input type="submit">
</form>
</body>
</html>
```
![Untitled (7)](https://user-images.githubusercontent.com/67935853/105051397-0df87f80-5ab2-11eb-85bc-f1b93c228a68.png)

- 문자 입력

```html
<html><<body>
<form action="">
<p>text:<input type="text" name = "id" value="default value"></p>
<p>password: <input type="password" name ="pwd" value="default value"></p>
<p>textarea:
<textarea rows="2" cols="50">default value</textarea>
</p>
</form>
</body></html>
```
![Untitled (8)](https://user-images.githubusercontent.com/67935853/105051428-1650ba80-5ab2-11eb-92f4-c08a42ce73a1.png)

- dropdown list

```html
<html>
<head><meta charset="utf-8">
</head>
<body>
<form action="[http://localhost/color.php](http://localhost/color.php)">
<h1>색상</h1>
<select name = "color">
<option value="red">붉은색</option>
<option value="black">검은색</option>
<option value="blue">파란색</option>
</select>
<h1>색상2(다중 선택)</h1>
<select name = "color2" multiple>
<option value="red">붉은색</option>
<option value="black">검은색</option>
<option value="blue">파란색</option>
</select>
<input type="submit">
</form>
</body>
</html>
```

![Untitled (9)](https://user-images.githubusercontent.com/67935853/105051446-1cdf3200-5ab2-11eb-9fc3-bef7d1e01e42.png)

- radio,checkbox

```html
<html>
<head>
<meta charset="utf-8">
</head>
<body>
<form action="[http://localhost/order.php](http://localhost/order.php)"
<p>
<h1>색상(단일 선택)</h1>
붉은색: <input type="radio" name="color" value="red">
검은색: <input type="radio" name="color" value="black" checked>
파란색: <input type="radio" name="color" value="blue">
</p>
<p>
<h1>사이즈(다중 선택)</h1>
95: <input type="checkbox" name="size" value="95">
100: <input type="checkbox" name="size" value="100" checked>
105: <input type="checkbox" name="size" value="150" checked>
</p>
<input type="submit">
</body>
</html>
```
![Untitled (10)](https://user-images.githubusercontent.com/67935853/105051486-27013080-5ab2-11eb-95ff-e312f826b267.png)


- 버튼

```html
<html>
<head>
<meta charset="utf-8">
<body>
<form action="[http://localhost/form.php](http://localhost/form.php)">
<input type="text">
<input type="submit" value="전송">
<input type="button" value="버튼" onclick="alert('hello world')">
<input type="reset">
</form>
</body>
</head>
</html>
```
![Untitled (11)](https://user-images.githubusercontent.com/67935853/105051517-2d8fa800-5ab2-11eb-9722-23798e36b41c.png)

- hidden

UI가 없지만 서버로 어떤 값을 전송하고 싶을 때 사용

```html
<html>
<head>
<meta charset="utf-8">
</head>
<body>
<form action="[http://localhost/hidden.php](http://localhost/hidden.php)">
<input type="text" name="id">
<input type="hidden" name="hide" value="egoing">
<input type="submit">
</form>
</body>
</html>
```

- label

```html
<html>
<body>
<form action="">
<p>
<label for="id_txt">text</label>:
<input id="id_txt" type="text" name = "id" value="default value">
</p>
<p>
<label for="password">password</label>:
<input id="password" type="password" name ="pwd" value="default value"></p>
<p>
<label>textarea:
<textarea rows="2" cols="50">default value</textarea>
</label>
</p>
</form>
</body>
</html>
```

- method

기본적으로 get방식으로 작동, 숨기고 싶으면 post

```html
<html>
<head>
<meta charset="utf-8">
</head>
<body>
<form action="[http://localhost/method.php](http://localhost/method.php)" method="post">
<input type="text" name="id">
<input type="password" name="pwd">
<input type="submit">
</form>
</body>
</html>
```

- 파일 업로드

```html
<html>
<head>
<meta charset="utf-8">
</head>
<body>
<form action="[http://localhost/upload.php](http://localhost/upload.php)" method="post" enctype="multipart/form-data">
<input type="file" name="profile">
<input type="submit">
</form>
</body>
</html>
```

![Untitled (12)](https://user-images.githubusercontent.com/67935853/105051563-397b6a00-5ab2-11eb-9843-9e045127cc1e.png)
