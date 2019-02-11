---
title: javascript / API / mermaid
search: true  
categories:
-   javascript
tags:
-   javascript
-   api
-  diagram
header:  
    actions:
    -   label: GitHub
        url: https://github.com/knsv/mermaid
    -   label: Document
        url: https://mermaidjs.github.io/
---

# mermaid
markdown 기반 flow chart, sequence / class diagram, gantt chart, git graph 등을 표현할 수 있는 API


## Flowchart [#](https://mermaidjs.github.io/flowchart.html)

```mermaid
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```

## Sequence Diagram[#](https://mermaidjs.github.io/sequenceDiagram.html)

```mermaid
sequenceDiagram
    Alice->>John: Hello John, how are you?
    activate John
    John-->>Alice: Great!
    deactivate John
```


## Ganttchart[#](https://mermaidjs.github.io/gantt.html)
```mermaid
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section A section
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d
        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM5NjEzOTU3NywtMTIyMTM3ODc5MSwtOD
MzODA1NzU1LC0xODk4NjAxMzIzLC0xNDA3MTcxOTAyLDc4Mzgw
Nzk3OCwtODY1OTQzNzgwXX0=
-->