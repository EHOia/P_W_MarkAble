# 상표 출원 가능성 예측 서비스 
<br>

## **1️⃣  프로젝트 소개**

**유사군코드**와 **상표명**을 **입력**했을 때, 같은 상품의 상표명 데이터 내에서 **유사도가 높게 나타나는 상표명들**과 **가장 높은 유사도 확률**을 확인해 원하는 상표명이 출원 가능한지 판단할 수 있는 웹 서비스를 구축한다. 이후 추가적인 검색 옵션을 제공할 예정이다.

<br>

## **2️⃣  시스템 아키텍쳐**

![image](https://user-images.githubusercontent.com/75110752/126591637-493beb19-749e-4307-83f0-9a0eda6ed079.png)

## **3  설치**

a. 도커 설치.
[공식 사이트](https://docs.docker.com/engine/install/)의 가이드를 따라서 도커를 설치한다.

b. 이 Repository를 Clone 한다.
```shell
git clone https://github.com/2021-summer-program/Trademark_verification
```
c. Kipris API KEY 세팅.

1. 회원가입을 통해 API키 발급.
2. [이 사이트](https://plus.kipris.or.kr/portal/bbs/view.do?bbsId=B0000004&nttId=683&menuNo=200019)를 참조하여 API 활용 신청.
3. [kipris plus](https://plus.kipris.or.kr/portal/main.do) 메인페이지 데이터서비스 -> OpenAPI -> 상표출원속보 API 신청
4. backend/codes/api_key.txt 파일생성후, api_key.txt에 본인의 REST API KEY 복사해서 붙여넣기.

d. 실행

1. docker-compose build (최초 실행시에만)
2. docker-compose up 

