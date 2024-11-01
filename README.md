# javascript-lotto-precourse

## 1. 로또 구입 금액 받기

- [ ] 로또 구입 금액 받기

  - [ ] 1,000원 단위로 입력 받기
  - [ ] 1,000원으로 나눠 나누어 떨어지지 않으면 예외 처리<br />
        `throw new Error("[ERROR] 구입 금액을 1,000원 단위로 입력해 주세요.")`

## 2. 로또 발행하기

- [ ] 로또 1장은 1,000원 이므로 로또 구입 금액을 1000으로 나눈 값 만큼 발행
- [ ] 1개의 로또를 발행할 때 1 ~ 45 사이 숫자 중 중복되지 않은 6개의 숫자 뽑기
  - [ ] 중복되지 않아야 하므로 Set을 사용하여 size가 6이 될때까지 반복문 돌리기
  - [ ] 6개 숫자은 출력해야 하므로 따로 저장 및 sort를 이용해 오름차순 정렬
- [ ] 발행된 로또를 각각 배열의 형태로 번호 출력

## 3. 당첨 번호 입력 받기

- [ ] 당첨 번호 입력 받기
  - [ ] 당첨 번호는 총 6개이며 쉼표(,)를 기준으로 구분
  - [ ] 당첨 번호가 6개가 아니거나 쉽표(,) 기준으로 구분 되어 있지 않으면 예외 처리<br />
        `throw new Error("[ERROR] 당첨 번호는 총 6개, 쉼표(,)로 구분하여 입력해 주세요.")`

## 4. 보너스 번호 입력 받기

- [ ] 보너스 번호 입력 받기
  - [ ] 1 ~ 45 사이의 숫자 입력 받기
  - [ ] 숫자 범위를 넘거나 숫자가 아닌 경우 예외 처리<br />
        `throw new Error("[ERROR] 1 ~ 45 사이의 숫자로 입력해 주세요.")`

## 5. 당첨 확인

- [ ] 1등부터 5등까지 당첨 순위 결정

  ```
  	- 1등: 6개 번호 일치 / 2,000,000,000원
  	- 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
  	- 3등: 5개 번호 일치 / 1,500,000원
  	- 4등: 4개 번호 일치 / 50,000원
  	- 5등: 3개 번호 일치 / 5,000원
  ```

  - [ ] 일치하는 번호 수에 따라 등수 결정
    - [ ] 5개의 번호가 일치한 경우 보너스 번호와 일치 여부 확인하여 일치하면 2등 일치 하지 않으면 3등 처리
  - [ ] 동률이 나오는 경우는..?
    - [ ] 특별한 조건이 없기 때문에 보통 동등하게 나누지만 이 경우 1명이 로또를 구매하는 경우라고 볼 수 있기 때문에 당첨수는 증가시키지만 금액은 1개 당첨과 같이 처리

## 6. 수익률 계산

- [ ] 소숫점 둘째 자리에서 반올림

## 7. 당첨 통계 출력

- [ ] 요구사항에 일치하는 형태로 결과 출력
