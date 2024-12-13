# SPRING 초기환경세팅

------

스프링 초기환경을 세팅해 보겠습니다.

## 1. JDK 설치

jdk를 설치하기 전에 jdk와 jre 차이점을 알아보겠습니다.

#### JRE : 자바 실행 환경
 - 자바 애플리케이션을 실행하기위한 최소의 실행 환경을 제공
#### JDK : 자바 개발 도구
 - JRE에서 제공하는 실행 환경뿐만 아니라 자바 개발에 필요한 여러 가지 명령어 그리고 컴파일러를 포함

--------------------



JRE는 최소 개발 환경을 제공하고 jDK는 실행환경 뿐 아니라 여러가지 명렁어 그리고 컴파일러가 제공되기 떄문에 JDK를 설치하겠습니다.

## 2. 개발환경 세팅

JAVA : JDK1.8 (1.8u_231)
  ( https://www.oracle.com/technetwork/java/javase/downloads/index.html )
  
Eclipse : Version: 2019-12 (4.14.0)
  ( https://www.eclipse.org/downloads )
  
Spring : Spring Tools 3 Add-On for Spring Tools 4 3.9.11.RELEASE
  ( Eclipse MarketPlace에서 STS 검색해서 다운로드 )
  
Tomcat : apache-tomcat-9.0.30
  ( https://tomcat.apache.org )
  
MariaDB : mariadb-10.2.14-winx64 
  ( https://downloads.mariadb.org/mariadb/10.2.14/ )
  
MySQL Workbench : mysql-workbench-community-8.0.18-winx64
  ( https://dev.mysql.com/downloads/workbench/ )

---------------------

## 3. Tomcat 설정

#### Apache와 Tomcat의 장단점

Apache와 Tomcat의 장단점을 알아보면서 Tomcat을 사용한 이유를 알아보겠습니다.



### APACHE 

#### 장점 
처리속도가 빠르다.
구조가 단순하다 ->비용 절감
트이터 트레픽 과부화에 강함

#### 단점
정적인 데어터만 처리 가능
다른 서비스와 상호작용 불가능
---------------------------

### TOMCAT

#### 장점
데이터 흐름이 유동적
DB 등 여러 서비스가 가능

#### 단점

APACHE에 비해 속도가 느림
부가적인 비용이 발생
트래픽 과부하에 약함














