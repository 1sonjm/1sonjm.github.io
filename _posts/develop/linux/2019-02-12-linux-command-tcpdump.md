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
    -   label: Wiki
        url: https://ko.wikipedia.org/wiki/Tcpdump
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
- **-w** _filename_
dump기록을 콘솔이 아닌 파일형태로 저장. 기록이 끝난뒤 파일로 저장
- **-U**  

- **-v**
구문 분석 및 인쇄 할 때 (약간 더) 자세한 출력을 생성하십시오. 예를 들어 IP 패킷의 수명, 식별, 총 길이 및 옵션이 인쇄됩니다. 또한 IP 및 ICMP 헤더 체크섬 확인과 같은 추가 패킷 무결성 검사를 가능하게합니다.
- **-vv**
더 자세한 출력. 예를 들어 추가 필드는 NFS 응답 패킷에서 인쇄되고 SMB 패킷은 완전히 디코딩됩니다.
**-vvv**
- 더 자세한 출력. 예를 들어 telnet **SB** ... **SE** 옵션이 모두 인쇄됩니다. 함께 **-X** 텔넷 옵션뿐만 아니라 진수로 인쇄됩니다.
- **-G** _rotate_seconds_
일정 주기로 반복하여 dump 기록 작성하며, **-w**와 함께 사용하면 해당 파일로 반복해서 덮어 씌워집니다.  **-c** _count_ 지정시 파일명이 _filename_._count_로 명명됩니다.
- **-c** _count_
지정한 수만큼 반복됩니다.
<!--stackedit_data:
eyJoaXN0b3J5IjpbODM0OTA5NzUsMTcxMjg4NzI3MywtNjU2Nz
U3NzM5XX0=
-->