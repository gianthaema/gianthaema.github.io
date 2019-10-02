---
layout: post
title:  "Disqus"
subtitle:   "댓글서비스"
author: 이종도
comments: true
---

## __Jekyll에 Disqus 적용 방법 - 댓글서비스__

## __1. Disqus?__

__Disqus__ 는 __소셜 댓글 서비스__ 의 하나로 다양한 SNS와 연동해서 댓글을 달 수 있습니다.  
별도의 댓글시스템을 구현할 필요없이 간단한 설정만으로 디스커스에서 제공하는 위젯을 사용할 수 있습니다.


## __2. Disqus 가입 및 설정__

1. __Disqus 가입__  
    [https://disqus.com/](https://disqus.com/)에서 __회원가입__ 을 하신 후에 __Email__ 인증을 합니다.<br>
    
2. 메인화면에서 __GET STARTED__ 를 누릅니다.<br>
![01.DISCUS](/assets/img/posts/2019-10-01-DISCUS/01.DISCUS.png) 
<br><br>

3. __I Want to install Disqus on my site__ 를 누릅니다.<br>
![02.DISCUS](/assets/img/posts/2019-10-01-DISCUS/02.DISCUS.png) 
<br><br>

4. Website Name, Category, Language 를 입력/선택합니다.  
   Website Name 의 경우 나중에 __Jekyll__ 에서 사용되는 설정 값 __Shortname__ 이 됩니다.  
   입력하신 이름이 중복인 경우 아래에 다음 예시와 같이 변경될 __Shortname__ 이 표시됩니다.  
   `예) Your unique disqus URL will be: gianthaema-8.disqus.com`<br>
![03.DISCUS](/assets/img/posts/2019-10-01-DISCUS/03.DISCUS.png) 
<br><br>

5. __무료버전__ 을 선택합니다.<br>
![04.DISCUS](/assets/img/posts/2019-10-01-DISCUS/04.DISCUS.png) 
<br><br>

6. __Jekyll__ 을 선택합니다.<br>
![05.DISCUS](/assets/img/posts/2019-10-01-DISCUS/05.DISCUS.png) 
<br><br>

7. ___config.yml__ 에 다음과 같이 disqus 설정을 합니다.  
`사용하시는 테마에 따라 설정 방법이 상이할 수 있습니다. 테마별 설명서를 참고해주세요. 아래 설정은 hydejack 테마입니다.`
```yaml
# disqus 설정
disqus: gianthaema
```
위 설정만 하시는 경우 댓글기능 사용을 원하는 글 상단에 `comments: true` 를 추가해서 사용해야합니다.  
모든 posts 에 댓글 기능을 사용하시려면 ___config.yml__ 에 아래 설정을 추가합니다.   
(테마에 따라 하지 않아도 되는경우가 있습니다.)
```yaml
defaults:
  - scope:
      type: posts
    values:
      comments: true
```


## __3. Disqus 한글 설정__

한글 설정이 되지 않았다면 아래 이미지에 표시한 부분들이 Disqus 에서 설정한 언어로 보일 것입니다.<br>
![06.DISCUS](/assets/img/posts/2019-10-01-DISCUS/06.DISCUS.png)
<br><br>

한글 설정을 하기위해 아래 이미지를 따라 General 설정 페이지에 접근합니다.<br>
1. 로그인된 메인페이지 오른쪽 상단에 `Admin` 클릭<br>
![07.DISCUS](/assets/img/posts/2019-10-01-DISCUS/07.DISCUS.png)
<br><br>

2. `Edit Settings` 클릭<br>
![08.DISCUS](/assets/img/posts/2019-10-01-DISCUS/08.DISCUS.png)
<br><br>

3. 생성한 댓글 서비스 클릭<br>
![09.DISCUS](/assets/img/posts/2019-10-01-DISCUS/09.DISCUS.png)
<br><br>

4. `General` 클릭 (아마 기본으로 General 페이지로 접근될 것입니다.)<br>
![10.DISCUS](/assets/img/posts/2019-10-01-DISCUS/10.DISCUS.png)
<br><br>

5. 언어 설정하는 부분을 `브라우저 개발자도구`를 사용하여 아무 언어의 `value` 를 `"ko"` 로 변경하신 후에 선택하여 저장합니다.<br>
![11.DISCUS](/assets/img/posts/2019-10-01-DISCUS/11.DISCUS.png)
<br>






