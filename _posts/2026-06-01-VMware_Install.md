---
title: "VMware 설치"
date: 2026-06-01
categories: 
  - Environment
  - Windows
tags: [Install, Virtualization]
---

## 🚀 [개요]
Windows 환경에서 가상화 실습을 위해 VMware Workstation을 설치하는 방법을 정리합니다.
설치 파일 실행부터 기본 설치 완료까지의 과정을 단계별로 진행합니다.

## 🔍 [VMware 설치]
1. VMware Workstation Pro 설치 마법사 화면이 나타나면 "Next" 버튼을 클릭합니다.
<img width="493" height="387" alt="image" src="https://github.com/user-attachments/assets/7031aa27-46cd-45cd-bb28-3dc77d1149a6" />

2. "I accept the terms in the License Agreement" 항목을 선택하여 라이선스 동의 후 "Next" 버튼을 클릭합니다.
<img width="496" height="395" alt="image" src="https://github.com/user-attachments/assets/a500d65c-17ca-4363-acf6-d5780da48a10" />

3. Compatible Setup 화면이 나타나면 현재 시스템에서 Hyper-V 또는 Device/Credential Guard 기능이 활성화되어 있음을 안내합니다.
   VMware를 사용하기 위해 "Install Windows Hypervisor Platform (WHP) automatically" 항목을 체크한 후 "Next" 버튼을 클릭합니다.

## ⚠️ [참고]

| 옵션 활성화 | 옵션 비활성화 |
|------|------|
| Hyper-V 위에서 WHP를 사용하여 VMware를 실행합니다. | Hyper-V를 비활성화 하지 않는 경우 Hyper-V가 가상화 기능을 점유하고 있어 VMware가 정상적으로 실행되지 않거나 기능이 제한될 수 있습니다. |


✅ 옵션 활성화
VMware 요청 
 ↓
WHP (API / 인터페이스 / 중계 역할)
 ↓
Hyper-V (가상화 담당)
 ↓
CPU (VT-x / AMD-V)

❌ 옵션 비활성화 (Hyper-V 활성화)
VMware 요청
↓
(직접 CPU 접근 시도 ❗)
↓
❌ Hyper-V가 막음 (이미 점유)

* WHP(Windows Hypervisor Platform)는 Hyper-V 기반 가상화 환경에서 VMware와 같은 애플리케이션이 가상화 기능을 사용할 수 있도록 지원하는 인터페이스(API)입니다. WHP를 사용하면 애플리케이션이 직접 CPU 가상화를 제어하지 않고, Hyper-V를 통해 가상화 기능을 사용하며 필요한 기능을 API 호출 방식으로 요청하게 됩니다.

<img width="496" height="395" alt="image" src="https://github.com/user-attachments/assets/315bdbd7-254e-4ae5-a666-d556c483040b" />

4. ㅇㄴ
5. 
   
