---
title: API 요청조절 / 스로틀링(Throttling), 디바운스(Debounce)
categories: 
  - network
tags: 
  - throttling
  - debounce
---

## 스로틀 (Throttle)
> 정해진 시간보다 많은 요청을 제한적 수용



## 디바운스 (Debounce)
> 연속적인 요청 발생 후 일정 시간 후 수용



## 버킷 알고리즘
FIFO 큐 형태로 패킷을 버킷에 담듯 쌓아서 처리 알고리즘에 따라 패킷제어
### 토큰 버킷 (Token bucket)
![https://i.imgur.com/XCfQQ0K.png](https://i.imgur.com/XCfQQ0K.png)
정해진 양의 토큰을 순환적으로 전달될 요청에 담아 토큰을 포함한 요청만 처리하는 패킷제어

소요시간 계산식
**time =  bucketSize ÷ (packetRate - tokenArrivalRate) × 1000m**

### 리키 버킷 (Leaky Bucket)
![Leaky Bucket](https://i.imgur.com/LYxD5V6.png)
최대 대역폭을 정해 일정한 요청이 발생하도록 패킷제어

초기값
> limit = 1000
> packet = [200, 700, 500, 450, 400, 200]

limit 을 초과하지 않는 패킷을 network로 전송
> limit = 1000 - 200 = 800
> packet = [200, 700, 500, 450, 400]
> limit = 1000 - 400 = 400
> packet = [200, 700, 500, 450]

pacaket[firstIn] > limit 인 경우, 절차 중단후 limit = 1000 으로 초기화 후 다음 절차 진행

소요시간 계산식
**time =  bucketSize × packetRate ÷ 1000m**

> 참조 
> - [https://webclub.tistory.com/607](https://webclub.tistory.com/607) - 디바운스(Debounce)와 스로틀(Throttle) 그리고 차이점 + 시연예제
> - [https://en.wikipedia.org/wiki/Throttling_process_(computing)](https://en.wikipedia.org/wiki/Throttling_process_(computing))
> - [https://docs.aws.amazon.com/ko_kr/apigateway/latest/developerguide/api-gateway-request-throttling.html](https://docs.aws.amazon.com/ko_kr/apigateway/latest/developerguide/api-gateway-request-throttling.html) - 처리량 향상을 위해 API 요청 조절
> - [https://12bme.tistory.com/504](https://12bme.tistory.com/504) - [성능] 스로틀링(Throttling)이란?
> - [https://www.zerocho.com/category/JavaScript/post/59a8e9cb15ac0000182794fa](https://www.zerocho.com/category/JavaScript/post/59a8e9cb15ac0000182794fa) -  쓰로틀링과 디바운싱
> - [https://www.slideshare.net/vimal25792/leaky-bucket-tocken-buckettraffic-shaping](https://www.slideshare.net/vimal25792/leaky-bucket-tocken-buckettraffic-shaping)

> Written with [StackEdit](https://stackedit.io/).

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA4NDQ3MDY1MF19
-->