# 숫자 야구 게임
## 진행 방법
* 숫자 야구 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 과제를 제출한다.

## 과제 제출 과정
* [과제 제출 방법](https://github.com/next-step/nextstep-docs/tree/master/precourse)

## 기능 목록
1. 게임 시작
- 게임을 시작하면 컴퓨터는 1 에서 9까지 서로 다른 임의의 수를 3개 선택한다.
2. 게임 진행
- 플레이어에게 입력을 받기 위해 `숫자를 입력해주세요 : `를 출력한다.
- 플레이어는 3개의 숫자를 입력한다.
  - 플레이어가 잘못된 값을 입력할 경우 에러 메시지를 출력하고 `게임 진행`의 첫번째 과정으로 돌아간다.
  - 에러 메시지는 `1. 1~9 범위를 벗어난 숫자를 입력`, `2. 입력한 길이가 3이 아닌 경우`, `3. 중복된 숫자를 입력한 경우`에 출력한다.
- 플레이어는 컴퓨터가 생각하고 있는 3개의 숫자를 입력하고, 입력한 숫자와 정답을 비교하여 점수를 산정한다.
    - 같은 수가 같은 자리에 있으면 `스트라이크`
    - 같은 수가 다른 자리에 있으면 `볼`
- 점수는 다음과 같은 형식으로 출력한다.
  - 산정한 점수는 기본적으로 `x스트라이크 x볼`의 형식으로 출력한다.
  - 스트라이크와 볼이 모두 0이라면 `낫싱`을 출력한다.
  - 스트라이크가 0이고 볼이 1이상이라면 `x볼`, 반대의 경우에는 `x스트라이크`의 형식으로 출력한다.
- 플레이어가 정답을 맞출때까지 위의 과정을 반복한다.
3. 게임 종료
- 플레이어가 정답을 맞추게 되면 `3개의 숫자를 모두 맞히셨습니다! 게임끝`을 출력한다.
- 플레이어에게 재시작 의사를 묻기 위해 `게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요.`를 출력한다.
- 플레이어가 `1`을 입력하면 `게임 시작` 단계로 돌아가며, `2`를 입력하여 게임을 종료할 수 있다.
  

