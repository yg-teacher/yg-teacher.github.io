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
### Step 1. 설치 마법사 시작
VMware Workstation Pro 설치 마법사 화면이 나타나면 "Next" 버튼을 클릭합니다.
<img width="493" height="387" alt="image" src="https://github.com/user-attachments/assets/7031aa27-46cd-45cd-bb28-3dc77d1149a6" />

### Step 2. 라이선스 동의
"I accept the terms in the License Agreement" 항목을 선택하여 라이선스 동의 후 "Next" 버튼을 클릭합니다.
<img width="496" height="395" alt="image" src="https://github.com/user-attachments/assets/a500d65c-17ca-4363-acf6-d5780da48a10" />

3. Compatible Setup 화면이 나타나면 현재 시스템에서 Hyper-V 또는 Device/Credential Guard 기능이 활성화되어 있음을 안내합니다.
   VMware를 사용하기 위해 "Install Windows Hypervisor Platform (WHP) automatically" 항목을 체크한 후 "Next" 버튼을 클릭합니다.

   ⚠️ [참고]
   | 구분 | 옵션 활성화 | 옵션 비활성화 (Hyper-V 활성화) |
   |------|-------------|-------------------------------|
   | 동작 방식 | WHP를 통해 Hyper-V 사용 | Hyper-V가 가상화 기능을 점유 |
   | CPU 가상화 접근 | 간접 사용 (WHP) | 접근 시도 → 실패 |
   | 실행 결과 | 정상 실행 | 실행 불가 또는 제한 동작 |
   
   ✅ 옵션 활성화 <br>
   VMware → WHP(API) → Hyper-V → CPU (VT-x / AMD-V)
   
   ❌ 옵션 비활성화 (Hyper-V 활성화) <br>
   VMware → (가상화 접근 시도 ❗) → Hyper-V 차단
   
   * WHP(Windows Hypervisor Platform)는 Hyper-V 기반 가상화 환경에서 VMware와 같은 애플리케이션이 가상화 기능을 사용할 수 있도록 지원하는 인터페이스(API)입니다. WHP를 사용하면 애플리케이션이 직접 가상화를 제어하지 않고, Hyper-V를 통해 가상화 기능을 API 호출 방식으로 요청하게 됩니다.
    
   * WHP(Windows Hypervisor Platform)를 사용하지 않는경우 원활한 사용을 위해 Hyper-V를 비활성화 합니다.
   <img width="496" height="395" alt="image" src="https://github.com/user-attachments/assets/315bdbd7-254e-4ae5-a666-d556c483040b" />

4. "Add VMware Workstation console tools into system PATH" 옵션은 VMware 관련 명령어를 명령 프롬프트(cmd)에서 경로 입력 없이 바로 사용할 수 있도록 환경 변수(PATH)에 등록하는 기능입니다. 해당 옵션은 사용 편의성을 높이기 위해 체크 상태를 유지한 후 "Next" 버튼을 클릭합니다.
   <img width="501" height="401" alt="image" src="https://github.com/user-attachments/assets/07fb3aff-b053-4dd4-a0f1-0f265f07859f" />
   
   ⚠️ [참고]
   * 해당 팝업 메시지는 VMware 설치 경로를 기본값이 아닌 위치로 변경했을 때 표시되며, 보안이 검증되지 않은 경로에 설치할 경우 파일 변조나 권한 상승(Privilege Escalation) 등의 보안 문제가 발생할 수 있음을 안내합니다. 이러한 이유로 기본 설치 경로 사용이 권장됩니다.
   <img width="547" height="221" alt="image" src="https://github.com/user-attachments/assets/1e2a6c54-3c37-434a-bacc-1ab5a3a0ffb6" />

   
5. VMware 설치 시 사용자 경험 개선을 위한 옵션을 설정하는 과정입니다. "Check for product updates on startup"은 VMware 실행 시 업데이트를 자동으로 확인하는 옵션이며, "Join the VMware Customer Experience Improvement Program"은 제품 개선을 위해 사용 데이터를 수집하는 기능입니다. 두 옵션은 비활성화하여도 VMware 사용에는 영향이 없으며, 필요에 따라 선택한 후 "Next" 버튼을 클릭합니다.
   <img width="627" height="502" alt="image" src="https://github.com/user-attachments/assets/13a3aa6f-f5c0-4978-9213-3c56e0108a9e" />

6. 해당 단계는 VMware Workstation의 바로가기(Shortcut) 생성 위치를 선택하는 옵션입니다.
   - Desktop: 바탕화면에 실행 아이콘 생성
   - Start Menu Programs Folder: 시작 메뉴에 프로그램 바로가기 등록

   두 옵션 모두 프로그램 실행 편의를 위한 기능으로, 기본 체크 상태를 유지한 후 "Next" 버튼을 클릭합니다.
   <img width="617" height="493" alt="image" src="https://github.com/user-attachments/assets/fa97fb1a-a10d-4657-8be7-ec6f61f45fb6" />

7. VMware Workstation Pro 설치를 시작하기 전 설정 내용을 최종 확인하는 화면으로서 수정이 필요한 경우 "Back" 버튼을 클릭하여 이전 단계로 이동할 수 있습니다. 특이상이 없는 경우 "Install" 버튼을 클릭하여 설치를 진행합니다.
   <img width="611" height="485" alt="image" src="https://github.com/user-attachments/assets/e2dde63b-0146-44d5-8be6-45dde58d7f3d" />

8. VMware Workstation Pro 설치 완료 후 "Finish" 버튼을 클릭하여 설치를 마무리합니다.
   <img width="615" height="492" alt="image" src="https://github.com/user-attachments/assets/5cc67d71-7fb2-44c1-8786-9d6aed0ed92b" />
   <img width="618" height="492" alt="image" src="https://github.com/user-attachments/assets/bef81d36-0622-42b4-a56a-b792f7a70f3c" />

## ✅ [결과]
Windows 환경 기준 VMware Workstation Pro 17.6.4 버전 설치를 완료했습니다.
