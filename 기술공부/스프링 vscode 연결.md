# SPRING <> VSCODE 연결



  스프링과 vscode를 연결해 보겠습니다.

### 1.확장프로그램 다운  


 - Extension Pack for Java

<img width="724" alt="스크린샷 2024-12-14 오후 4 27 17" src="https://github.com/user-attachments/assets/8dc1b311-3932-4aba-9683-c8206aaf5142" />

  
 - Gradle for Java

  <img width="714" alt="스크린샷 2024-12-14 오후 4 28 59" src="https://github.com/user-attachments/assets/c37dbd6c-e835-4773-b403-232c220aeae3" />


 - Spring Boot Extension Pack
 
  <img width="609" alt="스크린샷 2024-12-14 오후 4 29 49" src="https://github.com/user-attachments/assets/9d2d7308-beea-4420-8a83-b518fb3f6acd" />


### 2.프로젝트 생성

##### [command] + [Shift] + [P]  실행

----------------------------


<img width="606" alt="스크린샷 2024-12-14 오후 10 23 05" src="https://github.com/user-attachments/assets/ce575468-55f9-4b96-bf96-dc04ae69ed0b" />

-

<img width="601" alt="스크린샷 2024-12-14 오후 10 23 22" src="https://github.com/user-attachments/assets/e79d71b3-d97d-40f9-a147-2ddd1af40e5a" />

-

<img width="610" alt="스크린샷 2024-12-14 오후 10 23 29" src="https://github.com/user-attachments/assets/9aaa0ace-2ea6-49e6-859f-99b73d29a641" />

-

<img width="578" alt="스크린샷 2024-12-14 오후 10 23 35" src="https://github.com/user-attachments/assets/4accd49f-6fff-4d8e-b727-c5fb606d7019" />

-

<img width="586" alt="스크린샷 2024-12-14 오후 10 23 58" src="https://github.com/user-attachments/assets/d3bd7bcb-f9cf-4617-ba71-c8f79af282e0" />

-

<img width="597" alt="스크린샷 2024-12-14 오후 10 24 05" src="https://github.com/user-attachments/assets/92b795a4-2a33-47bd-a2af-f0d2295398e2" />

-

<img width="594" alt="스크린샷 2024-12-14 오후 10 24 11" src="https://github.com/user-attachments/assets/a0d966fa-19db-4904-a865-38c3b4ae90d6" />

-

<img width="587" alt="스크린샷 2024-12-14 오후 10 24 18" src="https://github.com/user-attachments/assets/21b07088-bec6-4083-b127-cc18102c8b50" />


-----

#### 순서대로 진행


후 코드 위치

<img width="749" alt="스크린샷 2024-12-14 오후 10 26 15" src="https://github.com/user-attachments/assets/3e33da93-c64d-4c3e-a4fa-83787b22df8f" />

src > main > java > com > project_s > project > ProjectApplication.java

여기에 코드 삽입

```

import org.springframework.web.bind.annotation.*;

@RestController
class Helloworld {
        @GetMapping("/")
        public String greet() {
                return "Hello!";
        }
}


```


---------------

그후 다음 명령어를 입려해서 gradle binary를 설치합니다.

```
./gradlew
```

설치가 완료되면


```
./gradlew bootRun

```





