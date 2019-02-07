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

## 기본 코드
```java
public static void main(String[] args) {
    List<Player> footballTeam = new ArrayList<>();
    Player player1 = new Player(59, "John", 20);
    Player player2 = new Player(67, "Roger", 22);
    Player player3 = new Player(45, "Steven", 24);
    footballTeam.add(player1);
    footballTeam.add(player2);
    footballTeam.add(player3);
 
    System.out.println("Before Sorting : " + footballTeam);
    Collections.sort(footballTeam);
    System.out.println("After Sorting : " + footballTeam);
}
```
```java
public class Player {
    private int ranking;
    private String name;
    private int age;  
    Player(int ranking, String name, int age){
	    // constructor
    }
    // getters, setters  
}
```

## Comparable
### 정의
**구현되는 클래스의 기본 정렬기준을 별도로 구현**  
 정렬 기준을 변경하기 위해 정렬대상에게 Comparable 인터페이스의 compareTo(Object obj) 를 구현한다. 해당 메서드에서 비교 대상의 개체가 인수로 전달되는 개체보다 작거나 같은지 또는 큰지 여부를 나타내는 숫자로 반환한다.
 
### 코드
```java
public class Player implements Comparable<Player> {
    @Override
    public int compareTo(Player otherPlayer) {
	    // ranking 값이 작은 순으로 정렬
        return (this.getRanking() - otherPlayer.getRanking());
    }
}
```
> Before Sorting : [John, Roger, Steven]  
> After Sorting : [Steven, John, Roger]

## Comparator
### 정의
기존에 Comparable의 compareTo로 구현된 것이 아닌 별도의 정렬기준을 적용할때
### 코드
```java
Collections.sort(footballTeam,  new Comparator<Point>() {
	  @Override
	  public int compare(Point p1, Point p2) { 위와 동일 }
	};
);
```

# 참조
https://www.baeldung.com/java-comparator-comparable
https://cwondev.tistory.com/15
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2OTczMjE3ODUsMjkwNDM1NTE0LC0xOT
U1MzE3MjQsLTE0MTkyMTU2MzEsMTI3MDUzNzI4OSw1NTY5ODA2
MjldfQ==
-->