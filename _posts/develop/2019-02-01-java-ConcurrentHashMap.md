---
title: "java / API / ConcurrentHashMap"
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
Thread-Safe 한 HashMap. null값을 허용하지 않음.

putIfAbsent(K,  V) 메소드가 존재
```java
ConcurrentHashMap<String, Integer> chm = new ConcurrentHashMap<>();
chm.put("key1", 0);
chm.putIfAbsent("key1",  1);
chm.putIfAbsent("key2",  -1);
```

프로젝트 개발중에 netty channel을 생성한걸 관리하는 맵으로 사용되고 있었다. 추가 정리해야되겠다
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY3MTY3MzM0NiwtOTk2MTIyOTQ0LDEwND
kxMjkxLC0yMDg1Njg3ODY0XX0=
-->