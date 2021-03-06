---
title: java / API / Thread-Safe Map
categories: 
  - java
tags: 
  - api
  - java
header:  
  actions:
    - label: java api
      url: "https://docs.oracle.com/javase/8/docs/api/?java/util/Comparator.html"
---

프로젝트 개발중에 netty channel을 생성한걸 관리하는 맵으로 사용되고 있었다. 

# ConcurrentHashMap
Thread-Safe 한 HashMap. null값을 허용하지 않음.

putIfAbsent(K,  V) 메소드가 존재. 대상 key가 존재할 경우 기존값을 반환하고 존재하지 않을 경우엔 설정값을 반환 
```java
ConcurrentHashMap<String, Integer> chm = new ConcurrentHashMap<>();
chm.put("key1", 0);
// 존재하는 key1 에 대하여 기존값인 0 사용
chm.putIfAbsent("key1",  1);

// 존재하지않는 key2 에 대하여 설정값인 -1 사용
chm.putIfAbsent("key2",  -1);
```

# Collections.synchronizedMap()
다른 map들도 thread-safe 하게 wrapping 하여 사용할 수 있습니다.
```java
Collections.synchronizedMap(new  HashMap<Long, String>());  
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc1MjczMzcwNV19
-->