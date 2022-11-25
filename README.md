# 프로젝트
## 맥 OpenJDK 설치
```
brew install openjdk@17
sudo ln -sfn /opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk-17.jdk
echo 'export PATH="/opt/homebrew/opt/openjdk@17/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```
## Spring Initializr
[Spring Initializr](https://start.spring.io/)
* Project: Gradle Project
* Language: Java
* Group: 도메인주소
* Artifact: 프로젝트식별이름
* Name: 편의상 Artifact와 동일
* Description: 프로젝트 설명
* Package name: Group.Artifact (자동완성)
* Packaging: Jar
* Java: 17 (LTS)
* Dependencies
  * Spring Web
    * Spring MVC 개발 모델 및 Tomcat을 내장 컨테이너로 지원
  * Thymeleaf
    * 템플릿 엔진
  * Lombok
    * 반복되는 코드를 애노테이션(@)을 이용해 간편하게 작성 지원
  * Spring Configuration Processor
    * application.yml 또는 application.properties의 값을 읽어와 멤버 변수에 자동 할당해주는 @ConfiguraionProperties 애노테이션 지원
  * Spring Boot DevTools
    * 애플리케이션 빠른 재시작 및 각종 설정 지원
# IntelliJ 설정
## 터미널 폰트 색상
라이트모드 테마 이용 시 터미널에 OMZ 테마 때문에 폰트가 안 보이는 문제
* Editor > Color Scheme > Console Colors
  * ANSI colors: Black
    * Foreground: **333333**
    * Background: **EEEEEE**
## Gradle 대신 IntelliJ 직접 빌드
* Build, Execution, Deployment > Build Tools > Gradle
  * Build and run
    * Build and run using: **IntelliJ IDEA**
    * Run tests using: **IntelliJ IDEA**
## Lombok Requires Annotation Processing
* Do you want to enable annotation processors?: Enable
# 뷰 리졸버
## 정적 페이지
* Welcome page

## 동적 페이지

## JSON
