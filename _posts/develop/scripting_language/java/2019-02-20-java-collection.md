---
title: java / API / Collection(List, Set), Map
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
# Collection
```mermaid
classDiagram
Iterable <|-- Collection
Collection <|-- Set
Set <-- AbstractSet
AbstractSet <|-- HashSet
HashSet <|-- LinkedHashSet
Set <|-- SortedSet
SortedSet <|-- NavigableSet
HashSet <|-- TreeSet

Collection <|-- List
List <-- AbstractList
List <|-- ArrayList
List <|-- Vector
Vector <|-- Stack
List <|-- AbstractSequentialList
AbstractSequentialList <|-- LinkedList
Deque <-- Deque
```

## List
## Set
# Map

# 참조
- https://dzone.com/articles/java-collections
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTgyMTQzMDYzMywxNDkxNTcwMTg0LDEyOT
AzNDM3NjQsMzMwNjM0NDI4XX0=
-->