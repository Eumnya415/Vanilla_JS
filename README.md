# Vanilla_JS
바닐라 자바스크립트 개인 스터디 Repo

# 공부 일지
## 24.02.22.
### 자바스크립트 작성 위치
* 첫 번째 유형 : head 태그에 script 태그를 만들어서 태그 안에 작성
  - 자바스크립트 코드를 head 태그 안에 작성하면 브라우저가 body 태그의 HTML 코드를 실행하기 전에 자바스크립트 코드를 먼저 해석하게 된다.
  - head 태그 안에 구현된 자바스크립트 코드가 많다면 브라우저는 자바스크립트 코드를 모두 해석한 이후에 HTML 코드를 실행하기 때문에 사용자에게 보이는 웹 페이지는 느려질 수 있다.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script>
        // 첫 번째는 head 태그에 script 태그를 만들어서 태그 안에 작성할 수 있다.
        document.write('자바스크립트 head에 위치<br>');
        // html 파일을 브라우저에서 열면, 브라우저 화면에 '자바스크립트 head에 위치'라는 문자열이 보이게 된다.
    </script>
</head>
<body>
    
</body>
</html>
```

<br>

* 두 번째 유형 : body 태그에 작성
  - body 태그에 있는 HTML 코드가 모두 실행되어 사용자가 보고 있는 브라우저 화면에 나타난 후 자바스크립트 코드를 실행함으로써 사용자가 느끼는 페이지의 로딩 속도를 높일 수 있다.
  - HTML의 코드를 실행시키기 위해 반드시 먼저 작성되어야 하는 JS 코드 (HEAD에 작성)를 제외하고는 body 태그 제일 하단에 코드를 작성하는 것이 좋다.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- HTML 코드가 작성되는 곳 -->
    <script>
        document.write('자바스크립트 body에 위치<br>');
        // html 파일을 브라우저에서 열면, 브라우저 화면에 '자바스크립트 head에 위치'라는 문자열이 보이게 된다.
    </script>
</body>
</html>
```
