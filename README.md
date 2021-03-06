---
description: 여러대의 분산 서버에서 대량의 데이터를 처리하는 분산 메시징 시스템
---

# What is Apache Kafka?

## 카프카?

### 목적

대량의 데이터에 대해 

* 높은 처리량
* 실시간

### 특징

* 확장성 : 데이터 양에 따른 시스템 확장 가능
* 영속성 : 수신한 데이터를 디스크에 유지 가능
* 유연성 : 연계할수 있는 제품이 많음
* 신뢰성 : 데이터 분실에 대한 걱정이 없음



### 주요 구성 요소

* 브로커 \(broker\)
  * 데이터를 수신, 전달하는 서비스
* 메시지 \(message\)
  * 카프카에서 다루는 데이터의 최소 단위.
    * 로그의 한 줄
    * 센서 테이터
  * key, value 를 가짐
  * 파티셔닝에 이용
* 프로듀서 \(producer\)
  * 데이터의 생산자
  * 브로커에게 메세지를 보내는 애플리케이션
* 컨슈머 \(consumer\)
  * 브로커에서 메시지를 취득하는 애플리케이션
* 토픽 \(topic\)
  * 메시지를 종류\(토픽\)별로 관리하는 스토리지
  * 브로커에 배치되어 관리됨
  * 프로듀서, 컨슈머는 특정 토핑을 지정하여 메시지 송수신
    * 단일 카프카 클러스터에서 여러 종류의 메세지 중계



### 주키퍼



+ 토픽, 파티션, 레플리카 개념 

+ 메시지 전송 시 파티셔닝 

- 라운드로빈에 의한 송신









