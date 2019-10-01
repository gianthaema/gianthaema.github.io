---
layout: post
title:  "highlight.js"
subtitle:   "코드문법강조"
comments: true
---

## __Highlight.js - 코드문법강조__

## __1. highlight.js?__

highlight.js 는 자바스크립트로 만든 코드 구문 강조를 위한 라이브러리로 어떠한 프레임워크에도 의존하지 않고, 거의 모든 마크업에서 작동하며 자동 언어 감지기능을 갖고 있습니다.

아래와 같이 원하는 구문을 박스에 보여줍니다.

```java
System.out.println("Hello. World!!")
```

* [highlight.js 다운로드 링크](https://highlightjs.org/download/)

* [highlight.js 스타일 데모 링크 ](https://highlightjs.org/static/demo/)

* [highlight.js 사용 설명서 링크](https://highlightjs.readthedocs.io/en/latest/index.html)

  

## __2. highlight.js 적용__

__highlight.js__ 는 아래의 __cdnjs, jsdelivr, download__ 방식 중 선택하여 __<head>__ 에 넣어 적용하시면 됩니다.

* __cdnjs__

```html
<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.10/styles/default.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/9.15.10/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
```

* __jsdelivr__

```html
<link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@9.15.10/build/styles/default.min.css">
<script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@9.15.10/build/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
```

* __download__ - [여기](https://highlightjs.org/download/)에서 원하는 언어를 선택하여 다운로드 받습니다.

```html
<link rel="stylesheet" href="./css/androidstudio.css">
<script src="./js/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>
```

 

## __3. highlight.js 스타일 변경__

스타일을 변경하려면 [여기](https://highlightjs.org/static/demo/)에서 적용할 스타일을 확인한 후에 __default.min.css__ 파일명을 바꾸시면 됩니다.

 

## __4. highlight.js 기본 사용법__

자동으로 pre>code 를 찾아 구문 강조가 적용되며, 구문 강조를 사용하지 않으려면 __class="nohighlight"__ 를 지정하시면 됩니다.

```html
<!-- 구문 강조 사용 -->
<pre><code> ... <code><pre>

<!-- 구문 강조 사용 안함 -->
<pre><code class="nohighlight"> ... </code></pre>
```























