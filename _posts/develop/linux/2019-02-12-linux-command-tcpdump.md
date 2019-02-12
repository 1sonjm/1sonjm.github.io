---
title: Linux / command / tcpdump
categories: 
  - 학습
tags: 
  - linux
  - command
header:  
    actions:
    -   label: Document
        url: https://www.tcpdump.org/manpages/tcpdump.1.html
---
# tcpdump

## 사용법
>**tcpdump** [ **-AbdDefhHIJKlLnNOpqStuUvxX#** ] [ **-B**  _buffer_size_ ]  
>  
>[ **-c**  _count_ ] [ **-C**  _file_size_ ]  
>[ **-E**  _[spi@ipaddr](mailto:spi@ipaddr)  algo:secret,..._ ]  
>[ **-F**  _file_ ] [ **-G**  _rotate_seconds_ ] [ **-i**  _interface_ ]  
>[ **--immediate-mode** ] [ **-j**  _tstamp_type_ ] [ **-m**  _module_ ]  
>[ **-M**  _secret_ ] [ **--number** ] [ **--print** ] [ **-Q**  _in|out|inout_ ]  
>[ **-r**  _file_ ] [ **-s**  _snaplen_ ] [ **-T**  _type_ ] [ **--version** ]  
>[ **-V**  _file_ ] [ **-w**  _file_ ] [ **-W**  _filecount_ ] [ **-y**  _datalinktype_ ]  
>[ **-z**  _postrotate-command_ ] [ **-Z**  _user_ ]  
>[ **--time-stamp-precision=**_tstamp_precision_ ]  
>[ _expression_ ]

## OPTION
자주 사용될만한 것만 정리

- **-w** filename
dump기록을 콘솔이 아닌 파일형태로 저장. 기록이 끝난뒤 파일로 저장
- **-U**  
저장 시, 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA0NDQyMzkyNV19
-->