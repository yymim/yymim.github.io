---
layout: post
title:  "정보처리기사 - 통합구현"
date:   2024-07-11 06:00:00 +0300
image:  
tags:   정보처리기사
---

# 연계 방식

### 간접 연계
* 중간 매개체를 통해 구성 요소들이 통신하는 방식
* EAI - 기업에서 운영되는 서로 다른 플랫폼 및 애플리케이션들 간의 정보전달, 연계, 통합을 가능하게 해주는 솔루션
* ESB - 기업에서 운영되는 서로 다른 플랫폼 및 애플리케이션들 간을 하나의 시스템으로 관리 운영할 수 있도록 서비스 중심의 통합을 지향하는 아키텍쳐
* 웹 서비스 - 네트워크에 분산된 정보를 서비스 형태로 개방하여 표준화된 방식. WSDL / SOAP
* 소켓

###  직접 연계
* 구성 요소들이 적접적으로 서로 연결되어 있는 방식
* DB 링크
* DB 연결
* API/Open API
* JDBC - 데이터베이스에서 자료를 조회하거나 업데이트하기 위해서 자바에서 데이터베이스에 접속할 수 있도록 하는 자바 API
* 하이퍼 링크

----------------------------------------------------

# 내외부 연계 모듈 구현

### EAI
* Enterprise Application Intergration
* 기업에서 운영되는 서로 다른 플랫폼 및 애플리케이션 간의 정보를 전달, 연계, 통합이 가능하도록 해주는 솔루션
* 각 비즈니스 간 통합 및 연계성 증대, 효율성 및 확장성을 높임

### EAI 구축 유형
<ul>
  <li>포인트 투 포인트</li>
  <li>허브 앤 스포크</li>
  <li>메시지 버스</li>
  <li>하이브리드 - 그룹 내는 허브 앤 스포크 방식, 그룹 간에는 메시지 버스 방식 사용</li>
</ul>

### ESB 방식
* Enterprise Service Bus
* 미들웨어를 중심으로 각각 프로토콜이 호환할 수 있도록 애플리케이션의 통합을 __느슨한 결합__ 방식으로 지원하는 방식이다.

### 웹 서비스 방식
<ul>
  <li>HTTP - HTML문서를 송.수신 하기 위한 규칙들을 정의해놓은 표준 프로토콜</li>
  <li>Hypertext - 문장이나 단어 등이 링크를 통해 서로 연결된 네트워크처럼 구성된 문서</li>
  <li>HTML - 웹을 이루는 가장 기초적인 구성요소. 인터넷 웹 문서를 표현하는 표준화된 마크업 언어</li>
</ul>

### 웹 서비스 유형
* SOAP - HTTP, HTTPS, SMTP등을 사용하여 XML 기반의 메시지를 교환하는 프로토콜
* WSDL - 웹 서비스명, 제공 위치, 메시지 포맷, 프로토콜 정보 등 웹 서비스에 대한 상세 정보가 기술된 XML 형식으로 구현되어있는 언어이다.
* UDDI - 웹 서비스에 대한 정보인 WSDL을 등록하고 검색하기 위한 저장소로 공개적으로 접근, 검색이 가능한 레지스트리이자 표준

### IPC 방식
* Inter Process Communication
* 메시지 큐 - 프로세스 또는 프로그램 간에 데이터를 교환하는 통신 방법
* 공유 메모리 - 컴퓨터 환경에서 여러 프로그램이 동시에 접근 할 수 이쓴ㄴ 메모리
* 소켓 - IP주소와 Port번호가 합쳐진, 네트워크상에서 서버 프로그램과 클라이언트 프로그램이 통신할 수 있도록 해주는 교환 기술
* 세마포어 - 각 프로세스에 제어신호를 전달하여 순서대로 작업을 수행하게 하는 기법

### LOD
* Linked Open Data
* 누구나 자유롭게 활용하고 재생산할 수 있도록 개방한 데이터
