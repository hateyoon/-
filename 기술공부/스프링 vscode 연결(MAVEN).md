# SPRING <> VSCODE 연결 (MAVEN)

스프링과 vscode를 연결해 보겠습니다.

### 1.확장프로그램 다운

 - Lombok Annotations Support for VS Code

<img width="541" alt="스크린샷 2024-12-15 오후 10 36 14" src="https://github.com/user-attachments/assets/8cd58cf0-78b8-414e-b193-2617028460f5" />

### 2.프로젝트 생성

<img width="611" alt="스크린샷 2024-12-15 오후 10 38 06" src="https://github.com/user-attachments/assets/972a963f-efdf-419e-b622-120359d4da5e" />

-
<img width="495" alt="스크린샷 2024-12-15 오후 10 38 21" src="https://github.com/user-attachments/assets/6059fbae-160e-4faa-bcd3-cf9c4c8f29b4" />

-

<img width="511" alt="스크린샷 2024-12-15 오후 10 38 32" src="https://github.com/user-attachments/assets/acd90e98-6668-4f15-81bd-d3fec2046766" />

-

<img width="526" alt="스크린샷 2024-12-15 오후 10 38 44" src="https://github.com/user-attachments/assets/99d6630e-a984-48b1-9794-65e43f8e68b2" />

-

<img width="453" alt="스크린샷 2024-12-15 오후 10 40 13" src="https://github.com/user-attachments/assets/f18e4f4a-a2a6-40f3-9248-5886dc863f92" />

-

<img width="516" alt="스크린샷 2024-12-15 오후 10 40 33" src="https://github.com/user-attachments/assets/4687624d-7bcc-4cf1-bfac-bc07c8569579" />

-

<img width="615" alt="스크린샷 2024-12-15 오후 10 40 46" src="https://github.com/user-attachments/assets/f05eac69-002d-4d3f-b3fb-8720360c6668" />

-

#### 그후 아래에 툴들을 설치해 주겠습니다.

--------

1. Spring Boot DevTools
2. Lombok
3. Spring Configuration Processor
4. Spring Web
5. Spring Data JPA
6. H2 Database
7. Flyway Migration
8. PostgreSQL


### 3. 파일생성

 - demo/src/main/resources/application.yml 순서대로 수정

```
logging:
  level:
    "[org.springframework.web]": debug
```

 - demo/src/main/resources/static/index.html 생성

```
<html>
  <div>Welcome</div>
</html>

```


 - demo/src/main/java/web/GreetingController.java 생성


```
package web;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

import service.GreetingService;

@RestController
public class GreetingController {
    String result;
    
    @GetMapping("/greeting")
    public String greeting() {
        result = GreetingService.greeting();
        return result;
    }
}

```

 - demo/src/main/java/service/GreetingService.java 생성
  
```
package service;

import org.springframework.web.bind.annotation.RestController;

@RestController
public class GreetingService {

    public static String greeting() {
        return ""Please, Hot dog World~";
    }   
}

```


### 4. 서버실행






<img width="339" alt="스크린샷 2024-12-15 오후 10 57 47" src="https://github.com/user-attachments/assets/a17ebb3f-c77e-43f8-850e-d8de399f1bf8" />












