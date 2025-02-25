# MonSpring
> 도서 검색 엔진 최적화 프로젝트
# 팀원

|김연태|이창욱|안연일|
|:--|:--|:--|
|Backend|Backend|Backend|
# ⚒스택
<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=Java&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">&nbsp;<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/redis-A41E11?style=for-the-badge&logo=redis&logoColor=white">&nbsp;
<img src="https://img.shields.io/badge/bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white">&nbsp;
<img src="https://img.shields.io/badge/Chocolatey-011A6A?style=for-the-badge&logo=Chocolatey&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=CSS3&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Logstash-005571?style=for-the-badge&logo=Logstash&logoColor=white">&nbsp;
<img src="https://img.shields.io/badge/Kibana-005571?style=for-the-badge&logo=Kibana&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=Thymeleaf&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=for-the-badge&logo=Apache Tomcat&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=JSON&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/JSON Web Tokens-000000?style=for-the-badge&logo=JSON Web Tokens&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=Gradle&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/JetBrains-000000?style=for-the-badge&logo=JetBrains&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/QueryDSL-0769AD?style=for-the-badge&logo=jQuery&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Microsoft Excel-217346?style=for-the-badge&logo=Microsoft Excel&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/kakao login-FFCD00?style=for-the-badge&logo=kakao&logoColor=black">&nbsp;<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=Gmail&logoColor=white"><img src="https://img.shields.io/badge/Google Drive-4285F4?style=for-the-badge&logo=Google Drive&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Spring Security-6DB33F?style=for-the-badge&logo=Spring Security&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=Windows&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=for-the-badge&logo=Visual Studio Code&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/SSE-007ACC?style=for-the-badge&logo=SSE&logoColor=white">&nbsp;<img src="https://img.shields.io/badge/POI-A41E11?style=for-the-badge&logo=POI&logoColor=white"><br>
<br />
![ac](https://user-images.githubusercontent.com/90178632/207832166-6ff6ccac-b284-4aa6-a3ba-e3a61d42ab46.png)
# 기술 스택 & 라이브러리 사용 이유
|기술 스택| 사용 이유|
|:--|:--|
|Querydsl|동적 쿼리 작성이 편리하며 컴파일 시점에 문법오류를 쉽게 확인가능해서 사용|
|JWT|유저의 세션을 저장할 필요가없고 유저가 보낸 토큰만 확인하면 되기에 사용|
|Redis|인메모리 방식으로 빠른 조회와 생성이 가능하고 만료시간을 정할 수 있어서 리프레쉬 토큰 저장용으로 사용|
|Thyemleaf|java 템플릿 엔진으로 front 구현을 위해 사용|
|Mysql|오픈 소스 라이센스이며 크기가 큰 데이터도 빠르게 처리가 가능하기에 사용|
|SSE|서버 > 클라이언트 방향으로 이벤트 발생시 알림을 위해 사용|
|POI|대용량 데이터 수집 및 엑셀 출력을 위해 사용|
|Spring Scheduler	|정보나루의 Book Detail 데이터 Open API 활용하여 데이터 수집을 위해 사용|
|ELK <br/>(ElasticSearch + Kibana + Logstash)|RDB(MySQL) 인덱싱, 튜닝과 비정형 데이터 조회 속도의 차이를 직접 테스트 해보고 마이그레이션 자동화가 가능한지 검증, Data LifeCycle Policy(Hot,Warm,Cold 아키텍쳐 적용) 설정으로 쉽게 데이터 생명주기를 관리하기 위해 사용|
# 서비스 및 기능 구현 담당자
|담당자|기능 및 서비스|
|:--|:--|
|김연태|ElasticSearch Analyzer & Tokenizer & Fillter Setting<br/>Kibana Visualization<br/>Logstash Data Migration<br/>MySQL Indexing & Setting<br/>AOP Developer Mailing Service<br/>Method StopWatch Log Remain & View Service<br/>Member Login Log Search Service (LifeCycle Policy Set -HWC-)<br/>Cursor Based Infinity Scroll<br/>Native Query Based Search Service<br/>Pagination & Select Optimization<br/>Excel Input Service<br/>Login Service (Security + Jwt + OAuth peristalsis)|
|이창욱|Redis Setting<br/>QueryDSL Based Search<br/>AOP Developer Slack Messaging Service<br/>QueryDSL Based Search Service<br/>Library Search Service<br/>Insert Optimazation<br/>Book Rental SSE Messaging Service<br/>Excel Output Service<br/>CSS Basic Setting<br/>Refresh Token LifeCycle Manage|
|안연일|JMitter Server Stress Test (Concurrency Controll test)<br/>Concurrency Improve Procsess<br/>OpenAPI Data Input RDB Service<br/>BookDetail Scheduling Service<br/>BookDetail Search & Batch Service<br/>Book Rental Service<br/>Redis conjugation for BookDetail & Rental Service improved<br/>Front Basic Setting<br/>Login Keep Procsess (Using cookie)|
# Total Data Handling Count
|DB|ROWS|
|:--|:--|
|MySQL|16,618,783|
|ElasticSearch|16,368,130|
|Redis|ExpireTime 1 day : Not Remain|
# 메소드 별 개선 순서에 따른 최소 밀리초 평균 (검색 성능 개선 그래프)
![stopwatch](https://user-images.githubusercontent.com/57734102/208287510-e591c73c-8c64-48ee-b836-56bd39749c81.png)
<br/>
# PPT 자료
Google Slide : https://docs.google.com/presentation/d/1GfGGs1gcFe5A7Z5237Y35HammJH8AkTfFNaKlepLnbQ/edit#slide=id.gcb9a0b074_1_0


