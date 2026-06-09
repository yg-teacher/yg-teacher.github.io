---
title: "Visual Studio Code 설정"
date: 2026-06-08
categories: 
  - Environment
  - Windows
tags: [Setting, IDE]
---

## 🚀 [개요]
Windows 환경에서 개발을 위한 Visual Studio Code를 설정하는 방법을 정리합니다.

### ⚠️ [참고]
- Visual Studio Code 설정 이전 JDK 설치([JDK 설치 가이드](https://yg-teacher.github.io/posts/JDK_Download_Setting))를 완료 후 진행 부탁드립니다.

## 🔍 [Visual Studio Code 설정]
### Step 1. 확장(Extensions) 화면 이동
왼쪽 사이드바에서 확장 아이콘을 클릭하거나 "Ctrl + Shift + X" 단축키를 입력하여 확장 화면으로 이동합니다.
<img width="781" height="675" alt="image" src="https://github.com/user-attachments/assets/c5017e81-db6d-416b-b7cb-5eb76e3394ea" />

### Step 2. VSCode 한글 언어팩 설치
검색 결과 중 "Korean Language Pack for Visual Studio Code (Microsoft)" 확장을 선택한 후 "Install" 버튼을 클릭하여 설치를 진행합니다.
> 📌 동일한 이름의 다른 확장이 있을 수 있으므로, 반드시 Microsoft에서 제공하는 확장을 선택합니다.
> 📌 Korean Language Pack 검색 및 Install 버튼 위치
<img width="1436" height="511" alt="image" src="https://github.com/user-attachments/assets/3fca6f5a-f263-4c69-9308-30cb975f7400" />

### Step 3. 한글 언어 적용 및 VSCode 재시작
한글 언어팩 설치 후 우측 하단에 표시되는 "Change Language and Restart" 버튼을 클릭합니다.
<img width="735" height="380" alt="image" src="https://github.com/user-attachments/assets/eddc6df3-5205-4253-837f-4789e82b0aa0" />
> 📌 만약 해당 팝업이 보이지 않는다면 아래 방법으로도 적용할 수 있습니다.
> 1. "Ctrl + Shift + P"를 입력하여 명령 팔레트를 실행합니다.
> <img width="805" height="152" alt="image" src="https://github.com/user-attachments/assets/c62b8c39-da85-4a91-81bd-910a57feafda" />
> 2. "Configure Display Language"를 검색하여 선택합니다.
> <img width="837" height="198" alt="image" src="https://github.com/user-attachments/assets/f0d72c46-4725-4fcd-b117-a37e11d20da6" />
> 3. 언어 목록에서 "ko"를 선택합니다.
> <img width="777" height="155" alt="image" src="https://github.com/user-attachments/assets/94848cb9-b324-4985-bbdc-a002b3da34e8" />
> 4. 팝업화면에서 "Restart" 버튼을 클릭하여 VSCode를 재시작합니다.
> <img width="657" height="207" alt="image" src="https://github.com/user-attachments/assets/d94f2141-bde8-49ae-8ca0-200c984ace59" />

### Step 4. Java 확장팩 설치
확장(Extensions) 화면에서 "Extension Pack for Java" 확장을 검색합니다. 검색 결과 중 Microsoft에서 제공하는 확장을 선택한 후 "Install" 버튼을 클릭하여 설치를 진행합니다.
> 📌 Java 개발을 위한 필수 확장으로 자동완성, 디버깅, 빌드 기능 등을 제공합니다.
<img width="1275" height="338" alt="image" src="https://github.com/user-attachments/assets/917f7091-b889-493f-a7f9-1f729eba8e12" />

### Step 5. Spring Boot 확장팩 설치
확장(Extensions) 화면에서 "Spring Boot Extension Pack" 확장을 검색합니다. 검색 결과 중 VMware에서 제공하는 확장을 선택한 후 "Install" 버튼을 클릭하여 설치를 진행합니다.
> 📌 Spring 공식 개발사(VMware)에서 제공하는 확장으로 Spring Boot 프로젝트 생성, 실행, 디버깅을 쉽게 할 수 있도록 지원하는 확장입니다.
<img width="1440" height="590" alt="image" src="https://github.com/user-attachments/assets/c05ce0e3-529a-40c4-9104-a7b545fde865" />
> 📌 확장 설치 시 "게시자 신뢰 및 설치" 팝업이 표시될 수 있습니다.  
> 이는 확장 프로그램의 게시자를 신뢰할 것인지 확인하는 보안 안내입니다.  
> Spring Boot Extension Pack은 VMware(공식 개발사)에서 제공하는 확장이므로  
> 안전하게 "게시자 신뢰 및 설치" 버튼을 클릭하여 설치를 진행합니다.
<img width="625" height="402" alt="image" src="https://github.com/user-attachments/assets/70c381bf-5a4d-4b3e-add4-20dd0ffbfdfe" />

## ✅ [결과]
Windows 환경 기준 Visual Studio Code 설정을 완료했습니다.
