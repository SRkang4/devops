# 7주차 - Docker Compose

## 실습 내용

- Docker Compose를 이용하여 방명록 웹앱과 Redis를 함께 실행
- Redis를 이용하여 방명록 데이터를 저장
- volume을 사용하여 컨테이너를 재시작해도 데이터가 유지되는지 확인
- 같은 Compose 네트워크 안에서 web 컨테이너가 redis라는 이름으로 Redis에 접근하는 과정 확인
- .env 파일을 이용하여 Redis 비밀번호를 compose.yaml에서 분리
- healthcheck를 추가하여 Redis가 준비된 뒤 web 컨테이너가 실행되도록 설정
- web 컨테이너를 3개로 늘리는 scale 실습
- 여러 web 컨테이너의 포트 충돌 문제를 확인하고 nginx를 이용하여 요청을 분산하도록 구성
