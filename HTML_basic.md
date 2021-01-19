# HTML 기초

참고 : 생활코딩 - HTML 강의

### 1. 기술 소개

- Hyper Text : 하이퍼텍스트를 가장 중요한 특징으로 하는
- Mark Up : 마크업이라는 형식을 가진
- Language : 컴퓨터 프로그래밍 언어

### 2. 기본 문법

- 글씨체 강조하기

```html
<strong>자신의 힘</strong>
```

- 제목

```html
<h1>오늘의 명언</h1>
```

- 소제목

```html
<h2>오늘의 명언</h2>
```

### 3. 하이퍼텍스트와 속성

- 링크

```html
<a target = "_blank"  title="전설적인 프로그래머" href = "[https://](https://ko.wikipedia.org/wiki/%EB%8F%84%EB%84%90%EB%93%9C_%EC%BB%A4%EB%88%84%EC%8A%A4)">도널드 커누스</a>
```

### 4. 태그의 중첩과 목록

- 리스트 만들기

```html
<li>기술 소개</li>
<li>기본 문법</li>
<li>하이퍼텍스트와 속성</li>
<li>리스트와 태그의 중첩</li>
```

- 같은 그룹끼리 묶기

```html
<ul>
  <li>기술 소개</li>
  <li>기본 문법</li>
  <li>하이퍼텍스트와 속성</li>
  <li>리스트와 태그의 중첩</li>
</ul>
<ul>
  <li>홍혜림</li>
  <li>홍혜림</li>
  <li>홍혜림</li>
</ul>
```

- 순서가 있는 리스트

```html
<ol>
<li>기술 소개</li>
<li>기본 문법</li>
<li>하이퍼텍스트와 속성</li>
<li>리스트와 태그의 중첩</li>
</ol>
```

### 5. 문서의 구조

- 탭의 제목 달기

```html
<title>HTML - 수업소개</title>
```

- 글씨 깨짐 방지

```html
<meta charset="utf-8">
```

- 본문을 꾸며주는 태그

```html
<head>
<title>HTML - 수업소개</title>
<meta charset="utf-8">
</head>
```

- 본문

```html
<body>
<h1>HTML</h1>
<ol>
<li>기술소개</li>
<li>기본문법</li>
<li>하이퍼텍스트와 속성</li>
<li>리스트와 태그의 중첩</li>
</ol>
</body>
```

- 전체적인 구조

```html
<html>
<head>
<title>HTML - 수업소개</title>
<meta charset="utf-8">
</head>
<body>
<h1>HTML</h1>
<ol>
<li>기술소개</li>
<li>기본문법</li>
<li>하이퍼텍스트와 속성</li>
<li>리스트와 태그의 중첩</li>
</ol> 
<h2>선행학습</h2>
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</body>
</html>
```

### 6. DOCTYPE

- 문서 형식 정의

```html
<!DOCTYPE html>
```

### 7. 웹사이트 만들기

- index.html 만들기

```html
<html>
<head>
<title>HTML - 수업소개</title>
<meta charset="utf-8">
</head>
```

```html
<body>
<h1><a href="index.html">HTML</a></h1>
<ol>
<li><a href="1.html">기술소개</a></li>
<li><a href="2.html">기본문법</a></li>
<li><a href="3.html">하이퍼텍스트와 속성</a></li>
<li><a href="4.html">리스트와 태그의 중첩</a></li>
</ol>
<h2>선행학습</h2>
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</body>
</html>
```

![HTML%20%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20c82d642bd87347ad828256257b34295d/Untitled.png](HTML%20%E1%84%80%E1%85%B5%E1%84%8E%E1%85%A9%20c82d642bd87347ad828256257b34295d/Untitled.png)