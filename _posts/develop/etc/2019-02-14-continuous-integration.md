---
title: Continuous Integration
categories: 
  - etc
tags: 
  - ci
  - system
---
# Continuous Integration
CI(**C**ontinuous **I**ntegration), 지속적 통합이란 소스관리, 빌드, 배포 등의 구조를 자동화 함으로써 소프트웨어 개발에 위험을 줄이는 방법으로 사용되고 있습니다.

![Imgur](https://i.imgur.com/O4fkG4i.png)

## CI 구성의 핵심 4요소
### CI Server
빌드 스크립트를 작성하고 자동화 프로세스를 구성하여 빌드. 테스트를 포함한 자동화 절차를 통해 검증하며 오류를 감지한다.
예) `Jenkins`, `Travis` 등

### Source Control, Version Control
소스 코드 관리 및 팀 단위 구성의 프로젝트 진행시 필수적이며 오류 수정과정을 돕는다.
예) `Subversion(SVN)`, `Git`, `GitLab` 등

### Build Tool
Source Control에서 구성된 소스 코드를 실행 가능한 형태로 가공하며 사전에 구성된 테스트 절차를 진행하여 구성된 소스 코드의 결함을 파악한다.
예) `Maven`, `Gradle`, `Ant` 등

### Test Tool
사전 구성된 테스트 코드에 따라서 일련의 검증과정을 거친다. 기능의 검증 뿐만 아니라 코드 품질에 대해서도 검증과정이 진행되는것이 좋다.
예) `Junit`, `SonarQube` 등

## 개선을 위한


## 참조
- http://www.nextree.co.kr/p10799/


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1Mjk5MDAxMzMsLTcwNDgwNzc4NywxMj
g4ODMyMTM2LDM2MjI4MDc4NiwtMjEyMTA2MzAzNl19
-->