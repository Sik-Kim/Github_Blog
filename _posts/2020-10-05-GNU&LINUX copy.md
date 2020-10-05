---
title: HTTP Request message 구조
# cover-image: korea.jpg

# summary: GNU/LINUX 설명
---

## HTTP Request message 구조

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7fe5f60e-3866-48a0-abe7-cde61c0e001c/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7fe5f60e-3866-48a0-abe7-cde61c0e001c/Untitled.png)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b5bdd49-744c-49cc-ad01-16c82a11913d/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b5bdd49-744c-49cc-ad01-16c82a11913d/Untitled.png)

## Request Line (첫째 줄)

### Method : 웹브라우저와 웹서버가 어떤 방식으로 통신할 것인가

- GET : 리소스 획득(데이터를 웹서버로부터 가져올때 사용) - READ
- POST : 엔티티 전송 - UPDATE
- PUT : 파일 전송 - CREATE
- HEAD : 메시지 헤더 취득
- DELETE : 파일 삭제 - DELETE
- OPTIONS : 제공하고 있는 메소드의 문의
- TRACE : 경로 조사
- CONNECT : 프록시에 터널링 요구

### 1.html : 웹서버에 요청하는 정보가 무엇인가. (웹서버는 1.html 내용을 확인해서 웹브라우저 요청에 대해 응답한다.

### HTTP/1.1 : 웹브라우저가 현재 사용하고 있는 HTTP의 Version

## Request Header

### Host: localhost:8080

- Host : 인터넷에 연결되어 있는 컴퓨터 한대한대를 식별하는 이름
- [localhost:8080](http://localhost:8080) : 웹브라우저가 request 하는 웹서버의 주소를 나타냄
- 1개의 웹서버가 여러개의 호스트를 가지고 있을 수 있다.

    가령 1개의 웹서버가 a.com, b.com, [c.com](http://c.com) 3개의 사이트를 호스팅하고 있을때 각각의 [localhost](http://localhost) 주소는 다를 것이다. 이때 각각의 호스트는 가상호스트이다.

- 8080 : Port 번호(1대의 컴퓨터에는 여러개의 웹서버가 설치될 수 있는데 그것을 식별)

### User-Agent

- Web Browser의 다른 표현
- 현재 사용하는 웹브라우저, OS 정보를 전송함

### Accept-Encoding

- 웹브라우저가 지원하는 압축 방식을 나타냄
- 웹서버가 웹브라우저에게 네트워크 전송 효율을 위해 데이터를 압축해서 보내는 경우 이 정보를 필요로 함

### If-Modified-Since

- 웹브라우저가 현재 가지고 있는 정보의 마지막 다운로드 시간
- 즉, 가지고 있는 정보가 최신이라면 웹서버에게 반복해서 받는것을 방지할 수 있음