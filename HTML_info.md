# 정보로서 HTML

- 정보의 관점 html
- 디자인은 css

### 1. meta 태그

- 웹페이지를 설명해주는 태그

```html
<html>
<head>
<meta charset="utf-8">
<meta name="description" content="생활코딩의 소개자료">
<meta name="keywords" content="코딩,coding,생활코딩,프로그래밍">
<meta name="author" content="hyelim">
<meta http-equiv="refresh" content="30">
</head>
<body>
생활 코딩은 일반인에게 프로그래밍을 알려주는 온라인/오프라인 강의입니다.
</body>
</html>
```

### 2. 의미론적인 태그

```html
<html><head>
<title>HTML - 수업소개</title>
<meta charset="utf-8">
</head>
<body>
<header>
<h1><a href="index.html">HTML</a></h1>
</header>
<nav>
<ol>
<li><a href="1.html">기술소개</a></li>
<li><a href="2.html">기본문법</a></li>
<li><a href="3.html">하이퍼텍스트와 속성</a></li>
<li><a href="4.html">리스트와 태그의 중첩</a></li>
</ol>
</nav>
<section>
<article>
<h2>선행학습</h2>
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</article>
<article>
<h2>선행학습</h2>
본 수업을 효과적으로 수행하기 위해서는 웹애플리케이션에 대한 전반적인 이해가 필요합니다. 이를 위해서 준비된 수업은 아래 링크를 통해서 접근하실 수 있습니다.
</article>
</section>
<footer>
<ul>
<li><a href="privacy.html">개인보호정책</a></li>
<li><a href="about.html">회사 소개</a></li>
</ul>
</footer>
</body></html>
```
![Untitled (4)](https://user-images.githubusercontent.com/67935853/105050683-624f2f80-5ab1-11eb-8aca-e4bb263d350f.png)

