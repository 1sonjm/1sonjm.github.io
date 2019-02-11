---
title: javascript / API / mermaid
search: true  
categories:
-   javascript
tags:
-   javascript
-   api
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

<div class="mermaid">
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
</div>

## Sequence Diagram[#](https://mermaidjs.github.io/sequenceDiagram.html)

<div class="mermaid">
sequenceDiagram
    Alice->>John: Hello John, how are you?
    activate John
    John-->>Alice: Great!
    deactivate John
</div>

<script>
var config = {
    startOnLoad:true,
    theme: 'forest',
    flowchart:{
        useMaxWidth:false,
        htmlLabels:true
    }
};
mermaid.initialize(config);
window.mermaid.init(undefined, document.querySelectorAll('.language-mermaid'));
</script>
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzgzODA3OTc4LC04NjU5NDM3ODBdfQ==
-->