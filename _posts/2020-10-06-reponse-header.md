---
title: HTTP Response message 구조
# cover-image: korea.jpg

summary: HTTP Response message 구조
---

## Response message 구조

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/531f3af7-d493-4c7a-bc4e-ce85e79f9183/Untitled.png](https://www.notion.so/sikkim/Response-message-60e68d2160864696a813717722624115#8e8b896114f941c4a0323391e50e9a92)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78c220d0-68d2-4eaf-9ea8-ccb5905af5a9/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78c220d0-68d2-4eaf-9ea8-ccb5905af5a9/Untitled.png)

## Status

### HTTP/1.1 200 OK

- 1xx : 정보를 주기위한 응답
- 2xx : 통신 성공
- 3xx : 리다이렉션
- 4xx : 클라이언트 에러
- 5xx : 서버 에러

- 403 Forbidden : 요청한 리소스는 있으나 웹서버가 거부(User가 권한이 없을 때)
- 404 Not Found : 요청한 리소스가 없어 웹서버가 전송할 수 없음
- 500 Internal Server Error : Web Server 내부 문제로 전송이 불가할 때

### Last-Modified: Tue, 17 Jul 2018 23:28:26 GMT

- content의 마지막 수정 시간을 표시

### Content-Encoding: gzip

- content의 압축 방식 표시 (gzip으로 압축해서 response 함)

### Content-Length: 1434

- Content의 전체 크기 표시(Content의 전체 크기는 1434byte)

### Content-Type : text/html

- 웹서버가 응답할 때 text를 html 형태로 response 한 것
- 웹브라우저는 Content-Type에 맞춰 UI를 실행한다

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/340f735e-73ef-45c6-93fd-4f100e8bba15/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/340f735e-73ef-45c6-93fd-4f100e8bba15/Untitled.png)

## Response message 구조

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/531f3af7-d493-4c7a-bc4e-ce85e79f9183/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/531f3af7-d493-4c7a-bc4e-ce85e79f9183/Untitled.png)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78c220d0-68d2-4eaf-9ea8-ccb5905af5a9/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78c220d0-68d2-4eaf-9ea8-ccb5905af5a9/Untitled.png)

## Status

### HTTP/1.1 200 OK

- 1xx : 정보를 주기위한 응답
- 2xx : 통신 성공
- 3xx : 리다이렉션
- 4xx : 클라이언트 에러
- 5xx : 서버 에러

- 403 Forbidden : 요청한 리소스는 있으나 웹서버가 거부(User가 권한이 없을 때)
- 404 Not Found : 요청한 리소스가 없어 웹서버가 전송할 수 없음
- 500 Internal Server Error : Web Server 내부 문제로 전송이 불가할 때

### Last-Modified: Tue, 17 Jul 2018 23:28:26 GMT

- content의 마지막 수정 시간을 표시

### Content-Encoding: gzip

- content의 압축 방식 표시 (gzip으로 압축해서 response 함)

### Content-Length: 1434

- Content의 전체 크기 표시(Content의 전체 크기는 1434byte)

### Content-Type : text/html

- 웹서버가 응답할 때 text를 html 형태로 response 한 것
- 웹브라우저는 Content-Type에 맞춰 UI를 실행한다

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/340f735e-73ef-45c6-93fd-4f100e8bba15/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/340f735e-73ef-45c6-93fd-4f100e8bba15/Untitled.png)