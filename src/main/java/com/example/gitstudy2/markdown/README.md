# 소개. Blog Service
---------------------
- 블로그 검색과 관련된 서비스를 제공합니다.

# 빌드 결과물
------------------
- [결과물 다운로드](https://www.google.com)

# 환경 소개
--------------------
- JAVA 17
- Spring Boot 2.7.3
- Gradle 기반 빌드
- H2 인메모리
- JUnit, MockMvc,FixtureMonkey 기반 테스트 케이스 작성
- REST docs 기반 API 명세 작성

# module - application
--------------------------
- 도메인 엔티티, 입력 포트, 출력 포트, 그리고 서비스 로직이 포함되어 있습니다.
  - `domain`
  - `service`
  - `port/input`
  - `port/output`

# module - adapter
--------------------
- 출력 포트에 대한 구현체가 포함되어 있습니다.
  - `adapter-persistence` (jpa)
  - `adapeter-http` (http-client)

# module - app
---------------------------
앱을 동작하기 위한 부분이 포함되어 있습니다.
- `app/app-api`

### 사용

> `$ http GET http://localhost:8080/api/v1/blogs?keyword=SpringFramework`


### 요청

Parameter

| Name    | Type | Description | Required |
---------|------|-------------|---------|
| `keyword` | `String` | 검색 키워드 | O       |
| `Url`     | `String`| 블로그 url | X|


