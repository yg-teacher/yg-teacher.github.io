title: "JDK 설치 및 환경변수 설정"
date: 2026-06-08
categories: 
  - Environment
  - Windows
tags: [Setting, JAVA]
---

## 🚀 [개요]
Windows 환경에서 개발을 위한 JDK 21 설치 및 환경변수 설정하는 방법을 정리합니다.

## 🔍 [JDK 다운로드 및 설정]
1. OpenJDK 공식 홈페이지(https://openjdk.org)에 접속한 후 좌측 메뉴에서 "JDK" 항목을 클릭합니다.
<img width="893" height="657" alt="image" src="https://github.com/user-attachments/assets/613a0970-1357-476d-9c42-fedc4a9312ca" />
<img width="842" height="920" alt="image" src="https://github.com/user-attachments/assets/794baa29-4d49-46d3-83a3-1fbcb068e9d1" />

2. 화면 중앙의 "Releases" 항목에서 "21 (GA 2023/09/19)"를 클릭합니다.
<img width="931" height="578" alt="image" src="https://github.com/user-attachments/assets/05b369d4-7ca1-4d9d-8bd5-01c06e4510e4" />

3. 본문 설명 중 "available from Oracle" 링크를 클릭하여 다운로드 페이지로 이동합니다.
<img width="942" height="280" alt="image" src="https://github.com/user-attachments/assets/02ddabb9-09ec-4908-8686-950689f0bd8b" />

4. 이동된 페이지에서 JDK 21은 현재 최신 버전이 아니기 때문에 "OpenJDK Archive" 링크를 클릭합니다.
<img width="892" height="671" alt="image" src="https://github.com/user-attachments/assets/6bc5bfbe-e497-40ac-88c3-bdce6606acd5" />

5. Archive 페이지에서 JDK 21 항목을 찾아 다운로드를 진행합니다.
<img width="915" height="792" alt="image" src="https://github.com/user-attachments/assets/4de4f034-c4a5-41f2-8d7d-3c03c5a959d8" />
<img width="650" height="753" alt="image" src="https://github.com/user-attachments/assets/d4a342f7-e31f-43ee-8415-56001f9b0073" />

6. 다운로드한 "openjdk-21.0.2_windows-x64_bin.zip" 파일의 압축을 해제합니다.
<img width="1041" height="110" alt="image" src="https://github.com/user-attachments/assets/89fea31a-939b-45ee-8f48-38325766bf95" />

7. 압축 해제 후 생성된 폴더의 이름을 "jdk-21.0.2"에서 "jdk21"로 변경합니다.
<img width="628" height="72" alt="image" src="https://github.com/user-attachments/assets/a736108d-0e6d-4dba-8cb7-d35133b5d752" />
<img width="622" height="77" alt="image" src="https://github.com/user-attachments/assets/37c4bfa6-22d9-4403-8357-9528d9191580" />

8. "jdk21" 폴더를 원하는 위치(예: D:\ 또는 C:\Java)에 이동합니다.
<img width="830" height="295" alt="image" src="https://github.com/user-attachments/assets/a1a5921f-9c73-45c3-8013-341860bfc7dc" />

9. Windows 검색창에 "환경 변수"를 입력한 후 "시스템 환경 변수 편집"을 클릭합니다.
<img width="1062" height="1007" alt="image" src="https://github.com/user-attachments/assets/25b6b205-08be-403b-a5dc-50179ad09ac9" />

10. 시스템 속성 창의 "고급" 탭에서 하단의 "환경 변수(N)..." 버튼을 클릭합니다.
<img width="611" height="707" alt="image" src="https://github.com/user-attachments/assets/6d71877d-7ac9-47a3-b791-eb123291d7bd" />

11. 환경 변수 창의 "시스템 변수(S)" 영역에서 하단의 "새로 만들기(W)..." 버튼을 클릭합니다.
<img width="793" height="782" alt="image" src="https://github.com/user-attachments/assets/9180d5b1-cfc1-4371-b615-a5d21c7fab6e" />

12. 새 시스템 변수 창에서 변수 이름(N)에 "JAVA_HOME"을 입력하고, 변수 값(V)에 JDK 설치 경로(예: D:\jdk21)를 입력한 후 "확인" 버튼을 클릭합니다.
<img width="837" height="222" alt="image" src="https://github.com/user-attachments/assets/02166a2c-5053-4cdd-9f20-1ac5291c347a" />

13. 환경 변수 창의 "시스템 변수(S)" 영역에서 "Path" 변수를 선택한 후 하단의 "편집(I)..." 버튼을 클릭합니다.
<img width="792" height="782" alt="image" src="https://github.com/user-attachments/assets/0ddd8f92-651f-4d71-aab5-2ad66f495155" />

14. 환경 변수 편집 창에서 "새로 만들기(N)"를 클릭한 후, 생성된 항목에 "%JAVA_HOME%\bin"을 입력하고 "확인" 버튼을 클릭합니다.
<img width="675" height="667" alt="image" src="https://github.com/user-attachments/assets/187e0783-ed27-47ba-8996-3ccf349ac2b7" />

15. 환경 변수 창과 시스템 속성 창에서 각각 "확인" 버튼을 클릭하여 설정을 저장하고 창을 닫습니다.
<img width="795" height="782" alt="image" src="https://github.com/user-attachments/assets/759314d7-79ef-40f0-8ad3-36a21dc4fff0" />
<img width="607" height="702" alt="image" src="https://github.com/user-attachments/assets/1ead7d6d-7112-45cd-9dd2-bfec2496060c" />


16. 


## ✅ [결과]
Windows 환경 기준 Visual Studio Code 설정을 완료했습니다.
