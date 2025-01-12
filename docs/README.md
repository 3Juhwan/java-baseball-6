# 구현할 기능 목록

### Application

어플리케이션의 전반적인 동작을 담당한다. 

- [x] 게임 시작 및 초기화
  - [x] Computer 인스턴스 생성
  - [x] MessageStream 시작 메시지 출력
- [x] 사용자 입력과 비교 로직 실행
  - [x] MessageStream 사용자 입력 안내 메시지 출력
  - [x] MessageStream 사용자 입력
  - [x] Computer 정답과 입력을 비교
  - [x] MessageStream 비교 결과 출력
  - [x] 예측 성공 시, 게임 재시작 로직으로 이동
- [x] 게임 재시작
  - [x] 게임 재시작 여부 메시지 출력
  - [x] 재시작 시, Computer 인스턴스 새로 생성
- [x] 예외 발생 시, 애플리케이션 종료

### MessageStream

콘솔을 통한 사용자와 상호작용을 담당한다. 입력 값을 검증하고, 적절한 메시지를 출력한다.

- [x] 메시지 출력
  - [x]  게임 시작 메시지 출력
  - [x]  사용자 입력 안내 메시지 출력
  - [x]  비교 결과 메시지 출력
  - [x]  게임 종료 메시지 출력
  - [x]  게임 재시작 여부 메시지 출력
- [x] 사용자 입력
  - [x] 사용자 입력
  - [x] 예외 발생 상황
    - [x] 사용자 입력의 길이가 3이 아닌 경우
    - [x] 사용자 입력에 숫자가 아닌 문자가 포함된 경우
    - [x] 범위 밖의 숫자가 포함된 경우

### Computer

숫자 야구의 정답을 생성하고 사용자 입력과 비교하는 역할을 담당한다. 게임마다 새로 생성된다. 

- [x] 인스턴스 생성과 동시에 새로운 정답 생성
- [x] 정답과 입력을 비교