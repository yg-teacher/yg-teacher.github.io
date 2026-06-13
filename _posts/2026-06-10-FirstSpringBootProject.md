---
title: "SpringBoot 프로젝트 생성"
date: 2026-06-10
categories: 
  - Environment
  - Windows
tags: [Project, SpringBoot, VScode]
---

## 🚀 [개요]
Windows 환경에서 Visual Studio Code를 사용하여 Spring Boot 프로젝트를 생성하는 방법과 실행 과정을 정리합니다.
### ⚠️ [참고]
- [Visual Studio Code 설정](https://yg-teacher.github.io/posts/VScode_Setting)을 완료 후 진행 부탁드립니다.

## 🔍 [SpringBoot 프로젝트 생성]
### Step 1. 명령 팔레트 실행
"Ctrl + Shift + P" 또는 "F1" 키를 입력하여 명령 팔레트를 실행합니다.
<img width="770" height="152" alt="image" src="https://github.com/user-attachments/assets/55efd0d4-a540-4af5-9e0d-a49dde944d05" />

### Step 2. Spring Initializr 선택
"Spring Initializr"를 검색하면 다양한 프로젝트 생성 및 확장 기능을 선택할 수 있으며 각 항목의 의미는 다음과 같습니다.

#### 1. Spring Initializr: Create a Maven Project...
Maven 기반의 Spring Boot 프로젝트를 생성합니다.
> 📌 pom.xml 파일 기반으로 프로젝트를 관리하며,  
> 📌 설정이 단순하고 입문자가 사용하기에 적합합니다.

#### 2. Spring Initializr: Add Starters...
이미 생성된 Spring Boot 프로젝트에 의존성(Starter)을 추가하는 기능입니다.
> 📌 프로젝트 생성 이후에도 DB, JPA, Security 등의 기능을 쉽게 추가할 수 있습니다.

#### 3. Spring Initializr: Create a Gradle Project with Kotlin DSL...
Kotlin DSL 기반의 Gradle 프로젝트를 생성합니다.
> 📌 build.gradle.kts 파일을 사용하며  
> 📌 Kotlin 문법으로 빌드 설정을 관리합니다. 

#### 4. Spring Initializr: Create a Gradle Project...
Gradle(Groovy DSL) 기반의 Spring Boot 프로젝트를 생성합니다.
> 📌 build.gradle 파일을 사용하며  
> 📌 Maven보다 빌드 속도가 빠르고 유연한 구성이 가능합니다.

Gradle 기반 프로젝트 생성을 위해 "Spring Initializr: Create a Gradle Project"를 선택합니다.
> 📌 Gradle을 선택한 사유로는 현업에서 가장 많이 사용되어 Gradle을 선택하였습니다
<img width="758" height="215" alt="image" src="https://github.com/user-attachments/assets/420d2813-af7e-47df-b9e0-0cae44eb95ea" />

### Step 3. Spring Boot 설정 정보 입력
Spring Initializr 실행 후 아래 정보를 순서대로 입력합니다.
- Spring Boot Version: 3.5.14
<img width="762" height="272" alt="image" src="https://github.com/user-attachments/assets/bc31fa15-83bb-4292-88a9-cd44745b16ec" />

- Language: Java
<img width="767" height="187" alt="image" src="https://github.com/user-attachments/assets/413a940c-a540-4e3d-96ec-b1c8de4e6598" />

- Group(기본 패키지 경로): com.example
<img width="765" height="127" alt="image" src="https://github.com/user-attachments/assets/fdf1afb3-1a5b-4298-bad8-69a0472ed3c5" />

- Artifact(메인 패키지 경로): demo
<img width="766" height="133" alt="image" src="https://github.com/user-attachments/assets/94dbf75e-6d4f-4bd3-8d0e-5ea73d98e49a" />

- Package Name(Group+Artifact): com.example.demo
> 📌 기본 패키지 경로로, Group과 Artifact를 기반으로 자동 생성됩니다.
<img width="762" height="127" alt="image" src="https://github.com/user-attachments/assets/bfd99c12-b422-4f74-bc1c-64b6fa3a95d3" />

- Packaging type: Jar
> 📌 Jsp를 사용한다면 War를 반드시 사용해야 하는 등의 규약이 있지만, 스프링 부트에서는 Jar를 권장하고 있습니다.
> 
> 📌 War는 외장 웹서버에 배포할 때 사용되며 Jar는 내장 서버를 포함하고 있어 별도의 서버 없이 실행 가능합니다. 
> 
> 📌 Jar: 자바 아카이브(Java Archive)의 약자로, 자바로 구현된 애플리케이션이 동작하는 데 필요한 클래스 파일, 라이브러리 파일을 포함하고 있습니다.
JRE(Java Runtime Environment)만 있어도 실행 가능합니다. 확장자는 .jar입니다.
> 
> 📌 War: 웹 아카이브(Web Archive)의 약자로, 웹 애플리케이션을 실행하는 데 필요한 리소스들의 압축 파일을 말합니다. jar파일의 일종으로, 자바 애플리케이션 중에서
웹 애플리케이션을 패키징하기 위한 파일입니다. 클래스 파일을 비롯해 JSP,서블릿(Servlet)등과 같이 웹 관련 파일등을 모두 포함할 수 있습니다. 
<img width="767" height="160" alt="image" src="https://github.com/user-attachments/assets/6e47a720-8a97-4415-8dda-33f26578454e" />

- Java Version: 21
<img width="757" height="212" alt="image" src="https://github.com/user-attachments/assets/9fb30a6a-37d0-40fa-a844-5cc6c4644abf" />

### Step 4. Dependencies 선택
의존성 선택 화면에서 검색창에 "Spring Web"을 입력한 후 해당 항목을 선택합니다.
선택이 완료된 상태에서 Enter 키를 입력하면 다음 단계로 진행합니다.
> 📌 "Spring Web"은 기본적인 웹 애플리케이션 실행을 위해 반드시 선택해야 합니다.
>
> 📌 여러 의존성을 선택할 수 있으며, 필요한 항목을 추가로 선택할 수 있습니다.
<img width="767" height="267" alt="image" src="https://github.com/user-attachments/assets/138af1b3-05cf-4068-881b-a8a1021f25ef" />
<img width="773" height="501" alt="image" src="https://github.com/user-attachments/assets/510f350b-822a-451e-87d3-3e3ad548435b" />

### Step 5. 프로젝트 생성 경로 선택
프로젝트를 생성할 폴더를 선택한 후 "Generate into this folder" 버튼을 클릭하여 프로젝트 생성을 진행합니다.
> 📌 선택한 폴더 내부에 Spring Boot 프로젝트가 생성됩니다.
> 
> 📌 새로운 폴더를 생성하여 관리하는 것을 권장합니다.
<img width="955" height="602" alt="image" src="https://github.com/user-attachments/assets/eb072976-20af-4cb3-a8c3-2f9a32fd35ed" />

### Step 6. 생성된 프로젝트 열기
프로젝트 생성 완료 후 좌측 하단에 나타난 팝업에서 "Open" 버튼을 클릭합니다.
이후 생성된 Spring Boot 프로젝트가 Visual Studio Code에 열립니다.
<img width="592" height="160" alt="image" src="https://github.com/user-attachments/assets/13dd1abd-996c-466c-864c-66c63015bbca" />
> 📌 프로젝트 생성 후 추가 설정 팝업이 표시될 수 있습니다.
> - Java 버전 업그레이드 안내: 현재 사용 중인 Java 버전(21)은 안정적인 버전이므로 "Not Now"를 선택합니다.  
> - Null 분석 기능: 코드의 null 오류를 사전에 확인할 수 있으므로 "Enable"을 선택하는 것을 권장합니다.
> <img width="575" height="317" alt="image" src="https://github.com/user-attachments/assets/e56ad5c5-410a-4309-b616-6a6d8089389f" />

### Step 7. Spring Boot 프로젝트 실행
프로젝트가 열리면 좌측 Explorer에서 메인 클래스 파일을 확인합니다.
일반적으로 아래 경로에 위치합니다.

"src/main/java/.../DemoApplication.java"

해당 파일을 열어 상단에 표시되는 "Run" 또는 "Debug" 버튼을 클릭합니다. 또는 아래 단축키를 사용하여 실행할 수 있습니다.
- Ctrl + F5 : 디버깅 없이 실행
- F5 : 디버깅 모드로 실행
<img width="1241" height="587" alt="image" src="https://github.com/user-attachments/assets/53bb5e53-23bf-4b2a-a7ed-b1f4404a3bda" />

### Step 8. 실행 결과 확인
Spring Boot 실행 후 브라우저에서 [Localhost](http://localhost:8080) 주소로 접속합니다.
> 📌 Whitelabel Error Page가 표시되더라도 정상적으로 서버가 실행된 상태입니다.
> 
> 📌 아직 '/' 경로에 매핑된 컨트롤러가 없기 때문에 표시되는 것으로, 서버 자체는 정상 동작 중입니다.
<img width="715" height="220" alt="image" src="https://github.com/user-attachments/assets/283374f0-069e-4705-bfb1-726ecdca197f" />

## ✅ [결과]
Windows 환경 기준 Visual Studio Code에서 Spring Boot 프로젝트 생성 및 실행이 정상적으로 동작하는 것을 확인하였습니다.

