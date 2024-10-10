
# Section 5. 스프링 부트 스타터와 라이브러리 관리

---

## 1. 라이브러리 직접 관리
- Spring Boot를 사용하지 않는 경우, 의존성 관리는 개발자가 직접 해야 합니다.
- 프로젝트에서 사용하는 라이브러리의 버전을 명시적으로 설정하고, 상호 호환성을 직접 관리해야 합니다.
- 이러한 방식은 라이브러리 간의 호환성을 수동으로 관리해야 하기 때문에 복잡해질 수 있습니다.

---

## 2. 스프링 부트 라이브러리 버전 관리
- Spring Boot는 **의존성 관리**를 자동으로 처리해 줍니다.
- Spring Boot BOM (Bill of Materials)을 사용하여 다양한 라이브러리의 호환 가능한 버전을 자동으로 관리합니다.
- Spring Boot의 BOM은 주요 라이브러리의 버전을 통합적으로 관리하므로, 호환성 문제를 줄여줍니다.
- 이를 통해 Spring Boot와 호환되는 안전한 버전을 사용할 수 있습니다.

---

## 3. 스프링 부트 스타터
- **Spring Boot Starter**는 특정 기능을 쉽게 통합할 수 있도록 도와주는 의존성 모음입니다.
- 여러 라이브러리를 개별적으로 관리할 필요 없이, 하나의 Starter로 관련된 라이브러리를 한 번에 설정할 수 있습니다.
- 예를 들어, **spring-boot-starter-web**은 웹 애플리케이션에 필요한 의존성(예: `Spring MVC`, `Jackson`, `Embedded Tomcat` 등)을 포함하고 있습니다.
- 사용 예시:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```
- Spring Boot Starter는 개발을 빠르고 쉽게 시작할 수 있도록 다양한 기능별로 제공됩니다.

---

**스프링 부트의 라이브러리 관리와 스타터 사용을 통해 개발자는 의존성 호환성을 쉽게 유지하고, 빠르게 필요한 기능을 애플리케이션에 통합할 수 있습니다.**
