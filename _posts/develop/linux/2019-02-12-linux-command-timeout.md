---
title: Linux / command / timeout
categories: 
  - 학습
tags: 
  - linux
  - command
header:  
    actions:
    -   label: Document
        url: https://linux.die.net/man/1/timeout
---
# timeout
프로세스를 설정된 시간동안 동작하도록 제한

## 사용법
> **timeout** [OPTION] NUMBER[SUFFIX] COMMAND [ARG]...  
> **timeout** [OPTION]

### NUMBER[SUFFIX]
실행하고자 하는 시간 입력. 기본 단위는 초(sec).
분은 m, 시간은 h로 사용한다
> timeout 3m  3 분
> timeout 1h  1시간

### [OPTION]
- -s, --signal=SIGNAL
specify the signal to be sent on timeout.
SIGNAL may be a name like 'HUP' or a number. See 'kill -l' for a list of signals
- --help
display this help and exit
- --version
output version information and exit
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNzMyMzY0MTZdfQ==
-->