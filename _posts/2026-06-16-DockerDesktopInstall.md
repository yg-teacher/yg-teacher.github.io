---
title: "Docker Desktop 설치"
date: 2026-06-16
categories: 
  - Environment
  - Windows
tags: [Install, Docker, kubernetes]
---

## 🚀 [개요]
Windows 환경에서 Docker Desktop을 설치하는 방법을 단계별로 정리합니다.  
Docker Desktop은 컨테이너 기반 개발 환경을 구성하는 도구로,  
로컬에서 Docker 및 Kubernetes 환경을 손쉽게 구성할 수 있습니다.


## 🔍 [Docker Desktop 다운로드 및 설치]
### Step 1. Docker Desktop 다운로드 화면으로 이동
https://www.docker.com 에 접속 후 상단 메뉴에서 "Products" → "Application Development" → "Docker Desktop"을 선택합니다.
<img width="1161" height="481" alt="image" src="https://github.com/user-attachments/assets/84a7d579-c0f3-431a-b0c3-d65242f49876" />

> 📌 아래 이미지와 같이 메뉴를 따라 이동하면 Docker Desktop 페이지로 진입할 수 있습니다.
> 
> ⚠ 처음 접속 시 상단 UI가 변경될 수 있으나, "Docker Desktop" 메뉴를 찾는 것이 핵심입니다.
<img width="1152" height="501" alt="image" src="https://github.com/user-attachments/assets/2eb119ad-6045-4612-b056-d186dccf9c2f" />

### Step 2. 운영체제에 맞는 Docker Desktop 다운로드
"Download Docker Desktop" 버튼에 마우스를 올리면 운영체제별 설치 파일이 표시된 목록에서 
자신의 환경에 맞는 항목을 선택하여 다운로드를 진행합니다.
> 📌 일반적인 Windows PC(인텔/AMD CPU)를 사용하는 경우 "Download for Windows - AMD64"를 선택하면 됩니다.
> 
> 📌 AMD64는 대부분의 PC에서 사용하는 표준 아키텍처이며, ARM64는 일부 특수 환경(예: ARM 기반 노트북)에서 사용됩니다.
> 
> ⚠ ARM64를 잘못 선택할 경우 Docker Desktop이 정상 실행되지 않을 수 있으므로 주의합니다.
<img width="1212" height="746" alt="image" src="https://github.com/user-attachments/assets/04e6b233-9e01-4a18-9ee2-7c8886e950a1" />


## ✅ [결과]
- 기존 1TB 디스크를 7:3 비율로 분할 완료
- 추가 파티션을 통해 독립적인 환경 확보
- 가상화 및 테스트 용도로 활용 가능

