---
title: "Visual Studio Code 설치"
date: 2026-06-08
categories: 
  - Environment
  - Windows
tags: [Install, IDE]
---

## 🚀 [개요]
Windows 환경에서 개발을 위한 Visual Studio Code를 설치하는 방법을 정리합니다.
설치 파일 실행부터 기본 설치 완료까지의 과정을 단계별로 진행합니다.

## 🔍 [Visual Studio Code 설치]
1. https://code.visualstudio.com 에 접근하여 Download 버튼을 클릭한 후, Windows 항목에서 User Installer (x64)를 선택하여 설치 파일을 다운로드합니다.
<img width="1588" height="483" alt="image" src="https://github.com/user-attachments/assets/588fb795-c52c-4364-b711-b03deabe1050" />
<img width="1552" height="696" alt="image" src="https://github.com/user-attachments/assets/5fe2b124-ec07-46cc-beb1-00555096754a" />

2. 다운로드 받은 설치파일을 실행합니다.
<img width="770" height="71" alt="image" src="https://github.com/user-attachments/assets/278fa0b8-d059-4729-b7cd-0d82a16738b5" />
   ⚠️ [참고]
   - 설치 파일 실행 시 다음과 같은 팝업이 나타날 수 있습니다.
   해당 메시지는 User Installer를 관리자 권한으로 실행했을 때 표시되는 안내입니다.  
   다만, 직접 관리자 권한으로 실행하지 않았더라도 Windows 계정이 관리자 권한을 가지고 있거나,
   시스템 환경에 따라 관리자 권한으로 자동 인식되는 경우에도 나타날 수 있습니다.
<img width="550" height="243" alt="image" src="https://github.com/user-attachments/assets/a9d8968b-1a66-403e-8917-642810900530" />

3. 라이선스 동의 화면에서 "동의합니다(A)"를 선택한 후 "다음(N)" 버튼을 클릭합니다.
<img width="692" height="567" alt="image" src="https://github.com/user-attachments/assets/0adfd2d5-1034-4aba-b4b5-9893874deae0" />

4. 설치 경로를 확인한 후 "다음(N)" 버튼을 클릭합니다.
<img width="690" height="562" alt="image" src="https://github.com/user-attachments/assets/e7d999b0-33d8-4423-b0d8-1c1f7c1ca77a" />

5. 시작 메뉴 폴더 생성 여부를 선택하는 화면입니다. 기본 설정을 그대로 사용할 경우 "다음(N)" 버튼을 클릭합니다. 
생성하지 않을 경우 "시작 메뉴 폴더를 만들지 않음(D)"을 체크한 후 "다음(N)" 버튼을 클릭합니다.
<img width="691" height="563" alt="image" src="https://github.com/user-attachments/assets/91f15c30-f553-4e65-84cc-c47d0642b9e8" />

6. 추가 작업 선택 화면에서 설치 시 적용할 기능을 선택합니다.
   각 옵션의 의미는 다음과 같습니다.
   - 바탕 화면에 바로가기 만들기(D)  
     → 바탕화면에 Visual Studio Code 실행 아이콘을 생성합니다. (선택 사항)
   - "Code(으)로 열기" (파일 컨텍스트 메뉴)  
     → 파일을 우클릭 했을 때 "Code로 열기" 메뉴가 추가됩니다.
   - "Code(으)로 열기" (디렉터리 컨텍스트 메뉴)  
     → 폴더를 우클릭 했을 때 "Code로 열기" 메뉴가 추가됩니다.
   - Code(을)를 지원하는 파일 형식에 대한 편집기로 등록  
     → 다양한 파일을 기본적으로 VS Code로 열 수 있도록 설정합니다.
   - PATH에 추가(다시 시작 후 사용 가능)  
     → 명령 프롬프트(cmd) 또는 PowerShell에서 `code` 명령어를 사용할 수 있도록 환경변수를 설정합니다.
     
   다음 항목은 체크하는 것을 권장합니다.
   - PATH에 추가 ✅  
   - 기본 편집기로 등록 ✅  
   - "Code로 열기" (파일/폴더) ✅  
   
   💡 특히 PATH 추가 옵션은 터미널에서 VS Code를 실행할 때 필요한 중요한 설정입니다.
   <img width="692" height="565" alt="image" src="https://github.com/user-attachments/assets/f636cfe7-a85b-4926-b191-f40f0ab811e0" />

7. 설치 내역을 확인한 후 "설치(I)" 버튼을 클릭하여 설치를 진행합니다.
<img width="692" height="562" alt="image" src="https://github.com/user-attachments/assets/e3d3bf01-d346-47c2-8e91-a7332339f5fa" />

8. 설치가 완료되면 "종료(F)" 버튼을 클릭하여 설치를 완료합니다.
<img width="688" height="565" alt="image" src="https://github.com/user-attachments/assets/ded06805-c1c8-415a-b6d9-bf826d73d3c3" />
<img width="690" height="560" alt="image" src="https://github.com/user-attachments/assets/411ab64a-c656-40a0-af03-3cc5101684a6" />

## ✅ [결과]
Windows 환경 기준 Visual Studio Code 설치를 완료했습니다.
