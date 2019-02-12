---
title: 알고리즘 / 버킷정렬
categories: 
  - algorithm
tags: 
  - algorithm
  - sort
---
인터넷 자료를 보던중 [컴퓨터의 세계 밖에서 발견한 O(n) 소팅](https://okky.kr/article/466103) 이란 게시글을 보게되었다.  

보통 정렬 알고리즘은 O(nlogn) 정도가 제일 빠른것으로 표를 통해 보았는데  
댓글중 버킷 정렬에 대한 댓글로 버킷정렬에 대해 얘기가 나와 궁금해졌다.

# 버킷 정렬(bucket sort)
## 절차

{% include figure image_path="https://i.imgur.com/I2HBqEx.png" alt="bucket sort progress" caption="bucket sort progress" %}

## 코드
```java
public void bucketSort(int[] numbers) {
	// int[0~9][0~n] 2차배열 생성
	List<LinkedList<String>> numberGroup = new ArrayList<>();
	for (int i = 0; i < 10; i++) {
	    numberGroup.add(new LinkedList<>());
	}

	// 맨앞자리 숫자값으로 분류하여 배열 삽입
	for (int num : numbers) {
	    String temp = Integer.toString(num);
	    int numIndex = Integer.parseInt(temp.substring(0, 1));
	    numberGroup.get(numIndex).add(temp);
	}

	// 배열 정렬
	for (LinkedList<String> numberList : numberGroup) {
        Collections.sort(numberList, Collections.reverseOrder());
	}
```

## 잡설
처음에 버킷정렬만 들었을 땐 감이 안왔는데 구조를 보자마자 생각난게  
알고리즘 풀이 시도중 K번째 수에 사용한 코드가 떠올랐다. 

버킷정렬을 고려하고 짠건 아닌데 이런 형태의 정렬구조가 있었음을 알았다.  
코드는 해당 풀이에서 가져왔는데 아마 더 나은 예시코드 가 있지않을까? 
사실 알게 모르게 다양한 정렬을 쓰고있을 것 이다.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMyMjE4Nzg0LC0xOTQwOTMxODkwXX0=
-->