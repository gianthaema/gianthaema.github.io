### 자이언트해마의 기술블로그 시작



#### 1. GitHub 블로그 만들기

1. 저장소 생성

2. Jekyll 테마 찾기

3. _config.yml 파일 가져와서 설정

4. index 파일 생성

5. _posts/ 경로에 새 글 작성

   

#####   참고 사이트

- 블로그 생성: [https://dreamgonfly.github.io/2018/01/27/jekyll-remote-theme.html](https://dreamgonfly.github.io/2018/01/27/jekyll-remote-theme.html)
- Jekyll 테마 적용: [https://github.com/mmistakes/minimal-mistakes](https://github.com/mmistakes/minimal-mistakes)
- 블로그 기본 설정: [https://devinlife.com/howto%20github%20pages/blog-config](https://devinlife.com/howto%20github%20pages/blog-config)



#### 2. 구글 애널리틱스 적용

1. 구글 애널리틱스 가입

2. 블로그 등 정보 입력

3. 발급된 추적ID를 _config.yml에 등록

   ```
   # Analytics
   analytics:
     provider               : "google-gtag" # 구글 애널리틱스 등록
     google:
       tracking_id          : "UA-134677596-2" # 추적ID
       anonymize_ip         : # true, false (default)
   ```



#####   참고 사이트

- 구글 애널리틱스: https://blogchannel.tistory.com/149
