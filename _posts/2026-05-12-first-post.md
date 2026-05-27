---
title: "Windows 파티션 나누기"
date: 2026-05-12
categories: 
  - Environment
  - Windows
tags: [Partition, Disk, DualBoot]
---

## 🚀 [개요]
Windows 환경에서 약 1TB 용량 디스크를 7:3 비율로 분할하여  
독립된 환경을 구성하는 방법을 정리합니다.

## 🔍 [운영환경]
- Windows 11 Pro
<img width="1251" height="322" alt="image" src="https://github.com/user-attachments/assets/0976b43c-2b25-40ef-9057-e2634ded0db8" />

- 로컬 디스크 용량

<img width="335" height="108" alt="image" src="https://github.com/user-attachments/assets/93ab8d68-96a6-45f5-a58e-a1cdba44f908" />

## 🛠 [파티션 분리 작업]
1. 키보드에서 Win + x 입력 후 "디스크 관리"를 선택합니다.<br>
<img width="262" height="737" alt="image" src="https://github.com/user-attachments/assets/bb813acf-0fba-43f4-adce-1cfbcad93f47" />
2. 디스크 관리 화면에서 C: 드라이브를 선택한 후 마우스 우클릭을 하고, 볼륨 축소를 선택합니다.
<img width="1022" height="892" alt="image" src="https://github.com/user-attachments/assets/b2d0b630-f192-4d0f-8524-00b76b1ed12f" />
3. 300GB 크기의 파티션을 분리하기 위해 "축소할 공간 입력(MB)" 항목에 307200을 입력 후 축소를 진행합니다.
<img width="945" height="750" alt="image" src="https://github.com/user-attachments/assets/40d8669b-907c-4c1e-adde-c2f334a8d263" />
4. 할당되지 않은 공간을 마우스 우클릭한 후 "새 단순 볼륨(New Simple Volume)"을 선택합니다.
<img width="938" height="743" alt="image" src="https://github.com/user-attachments/assets/ae91e4b5-8f2e-4b60-9a46-0050a991bc91" />
5. "다음" 버튼을 계속 클릭하여 진행한 뒤 마지막 단계에서 설정 내용을 확인하고 "마침"을 선택합니다.
<img width="942" height="745" alt="image" src="https://github.com/user-attachments/assets/09523554-11ed-4b54-a19d-e66fee451dac" />
<img width="938" height="742" alt="image" src="https://github.com/user-attachments/assets/acb8c7a3-1698-4c3a-bb79-81eb95658a87" />
<img width="942" height="747" alt="image" src="https://github.com/user-attachments/assets/00874bb1-a879-4534-8b9a-56c8443f552d" />
6. 디스크 관리 화면 및 "내 PC"에서 새로 생성된 파티션이 정상적으로 표시되는지 확인합니다.
<img width="937" height="746" alt="image" src="https://github.com/user-attachments/assets/2d5de50d-6380-4d42-bc5c-b76034f53adf" />
<img width="672" height="117" alt="image" src="https://github.com/user-attachments/assets/ad3f7dcd-1439-4df0-be69-973952721298" />

## ✅ [결과]
- 기존 1TB 디스크를 7:3 비율로 분할 완료
- 추가 파티션을 통해 독립적인 환경 확보
- 가상화 및 테스트 용도로 활용 가능

