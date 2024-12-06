# Postgresql 

----
- 자주쓰는 데이터베이스 중에 하나인 postgresql을 맥에서 환경설정 하는 법을 알아보려고 합니다.
----

저는 brew를 이용한 postgresql 설치하는 법을 공부했습니다.

```
brew update
```
먼저 brew를 최신정보를 가져오고 갱신합니다

```
brew install postgresql
```
로 다운을 받을 수 있다

#### 이때 

```
brew install postgresql@(내가 다운로드하고싶은 버젼) 을 입력하면 그버젼을 다운받을 수 있다.
```

다운로드가 잘 되었으면

```
psql postgres
```
명령어를 사용하면 데이터베이스로 접속할 수 있다.
