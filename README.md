# Codeit_파이썬(실습) 
## 실습1 _ 로또번호 자동생성 후 당첨금 확인 

#### 파일명 : lottary_play.py
#### 실행파일 : lottary.html

로또 시뮬레이션 프로그램을 만들어 보겠습니다.

이 프로그램은 과정이 많기 때문에, 여러 파트로 나눠서 문제를 해결해 나갈 건데요. 먼저 이 레슨에서 프로그램 전체에 대한 설명을 한 번 하고 가겠습니다.

#### 규칙
로또는 주 1회씩 열립니다. 하지만 한 사람이 한 회차에 여러 번 참여할 수도 있습니다.

번호는 1부터 45까지 있는데요. 주최측에서는 매주 6개의 '일반 당첨 번호'와 1개의 '보너스 번호'를 뽑습니다. 그리고 참가자는 1번 참여할 때마다 서로 다른 번호 6개를 선택합니다.


*당첨 액수는 아래 규칙에 따라 결정됩니다.*
1. 내가 뽑은 번호 6개와 일반 당첨 번호 6개 모두 일치 (10억 원)
2. 내가 뽑은 번호 5개와 일반 당첨 번호 5개 일치, 그리고 내 번호 1개와 보너스 번호 일치 (5천만 원)
3. 내가 뽑은 번호 5개와 일반 당첨 번호 5개 일치 (100만 원)
4. 내가 뽑은 번호 4개와 일반 당첨 번호 4개 일치 (5만 원)
5. 내가 뽑은 번호 3개와 일반 당첨 번호 3개 일치 (5천 원)

## 실습2 _ 숫자야구 게임

#### 파일명 : number_baseball.py

- '숫자 야구' 게임을 만들려고 합니다.

#### 규칙

- 컴퓨터는 0과 9 사이의 서로 다른 숫자 3개를 무작위로 뽑습니다. 예를 들어서 컴퓨터가 5, 2, 3을 뽑을 수도 있고 6, 7, 4를 뽑을 수도 있는 거죠.
- 사용자는 컴퓨터가 뽑은 숫자의 값과 위치를 맞추어야 합니다.
- 컴퓨터는 사용자가 입력한 숫자 3개에 대해서, 아래의 규칙대로 스트라이크(S)와 볼(B)의 개수를 알려줍니다.
1. 숫자의 값과 위치가 모두 일치하면 S입니다.
2. 숫자의 값은 일치하지만 위치가 틀렸으면 B입니다.
3. 예를 들어 컴퓨터가 1, 2, 3을 뽑았다고 가정합시다. 사용자가 1, 3, 5를 입력하면, 1S(1의 값과 위치가 일치) 1B(3의 값만 일치)입니다.
- 기회는 무제한입니다. 하지만 몇 번의 시도 끝에 맞췄는지 기록됩니다.
- 3S(숫자 3개의 값과 위치를 모두 맞춘 경우)가 나오면 게임이 끝납니다.

#### 진행 방식
1. "0과 9 사이의 서로 다른 숫자 3개를 랜덤한 순서로 뽑았습니다."가 출력됩니다.
2. "숫자 3개를 하나씩 차례대로 입력하세요."가 출력됩니다.
3. "1번째 숫자를 입력하세요: "가 출력되고, 사용자로부터 입력을 받습니다. 마찬가지로 "2번째 숫자를 입력하세요: "와 "3번째 숫자를 입력하세요: "가 출력되고, 사용자로부터 각각 입력을 받습니다. 만약 사용자가 중복되는 숫자를 입력하거나 범위에서 벗어나는 숫자를 입력하면, 사용자로부터 입력을 다시 받습니다.
5. 사용자가 올바르게 숫자 3개를 입력하면, 규칙에 따라 "*S *B"가 출력됩니다.
6. 3S가 아닌 경우, 2번부터 다시 진행합니다.
7. 사용자가 3S를 달성하면, "축하합니다. *번 만에 숫자 3개의 값과 위치를 모두 맞추셨습니다."가 출력됩니다. 그리고 게임은 종료됩니다.
