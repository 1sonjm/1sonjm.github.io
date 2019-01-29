---
title: "java / API / Comparable, Comparator"
search: true
categories: 
  - api
tags: 
  - api
  - java
header:  
  actions:
    - label: "java api"
      url: "https://docs.oracle.com/javase/8/docs/api/?java/util/Comparator.html"
---

# 핵심
객체가 정렬될때, 사용자의 의도에 따라 정렬 구조를 변경할 수 있도록 지원되는 인터페이스  

## Comparable
### 정의
구현되는 클래스의 기본 정렬기준을 별도로 구현
### 예시
```java
public class Player implements Comparable<Player> {
    @Override
    public int compareTo(Player otherPlayer) {
        return (this.getRanking() - otherPlayer.getRanking());
    }
}
```
>Before Sorting : [John, Roger, Steven]
>After Sorting : [Steven, John, Roger]
## Comparator
### 정의
기존에 Comparable의 compareTo로 구현된 것이 아닌 별도의 정렬기준을 적용할때
### 예시

# 참조
https://www.baeldung.com/java-comparator-comparable
https://cwondev.tistory.com/15
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg1NDc1MjU4MywxODc5NjM1NzM3XX0=
-->