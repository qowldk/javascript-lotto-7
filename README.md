# javascript-lotto-precourse

## 개요

이 프로그램은 콘솔 기반의 간단한 로또 발매기입니다. 사용자는 구입 금액을 입력하여 해당 금액만큼 로또를 구매하고, 당첨 번호와 보너스 번호를 입력하여 당첨 결과와 수익률을 확인할 수 있습니다.

## 기능

- **로또 발행**: 입력한 금액에 따라 로또를 발행합니다. 로또 한 장의 가격은 1,000원이며, 각 로또는 1부터 45 사이의 중복되지 않는 6개의 숫자로 구성됩니다.
- **당첨 번호 입력**: 당첨 번호 6개와 보너스 번호 1개를 입력받습니다. 모든 번호는 1부터 45 사이의 중복되지 않는 숫자여야 합니다.
- **당첨 결과 확인**: 구매한 로또와 당첨 번호를 비교하여 당첨 내역과 수익률을 계산하여 출력합니다.
- **에러 처리**: 잘못된 입력이 있을 경우 "[ERROR]"로 시작하는 메시지를 출력하고, 해당 단계부터 다시 입력을 받습니다.

## 당첨 기준 및 상금

| 등수 | 당첨 기준                        | 상금(원)      |
| ---- | -------------------------------- | ------------- |
| 1등  | 6개 번호 일치                    | 2,000,000,000 |
| 2등  | 5개 번호 일치 + 보너스 번호 일치 | 30,000,000    |
| 3등  | 5개 번호 일치                    | 1,500,000     |
| 4등  | 4개 번호 일치                    | 50,000        |
| 5등  | 3개 번호 일치                    | 5,000         |

1. - [x] 로또 구입 금액 입력받기

- [x] 1000원 단위가 아니면 예외 처리, 에러 문구 출력
- [x] 구입 금액이 입력되지 않았을 때 예외 처리, 에러 문구 출력
- [x] 구입 금액이 숫자가 아닐 때 예외 처리, 에러 문구 출력
- [x] 구입 금액이 0 일때 예외 처리, 에러 문구 출력
- [x] 구입 금액이 음수 일때 예외 처리, 에러 문구 출력

2. - [x] 금액에 맞게 로또 발행하기

- [x] 금액에 맞게 발행할 로또 수량 출력하기
- [x] 1개의 로또를 발행할 때 중복되지 않는 6개의 숫자 뽑기
- [x] 로또 번호는 오름차순 정렬하여 출력하기

3. - [x] 당첨 번호 입력받기

- [x] 번호는 쉼표(,)를 기준으로 구분
- [x] 숫자가 6개가 아니면 예외 처리, 에러 문구 출력
- [x] 모든 값이 숫자가 아니면 예외 처리, 에러 문구 출력
- [x] 숫자 범위 1 ~ 45 밖이면 예외 처리, 에러 문구 출력
- [x] 중복된 숫자가 있을 경우 예외 처리, 에러 문구 출력

4. - [x] 보너스 번호 입력받기

- [x] 숫자가 6개가 아니면 예외 처리, 에러 문구 출력
- [x] 숫자 범위 1 ~ 45 밖이면 예외 처리, 에러 문구 출력
- [x] 당첨 번호에 중복된 숫자가 있을 경우 예외 처리, 에러 문구 출력

5. - [x] 당첨 내역 출력하기

- [x] 사용자가 구매한 로또 번호와 당첨 번호 비교

6. - [x] 수익률 출력하기

- [x] 수익률은 소수점 둘째 자리에서 반올림

제약 사항

- indent depth 2 까지만 허용
- 3항 연산자 불가
- 함수는 한 가지 일만
- Jest 이용하여 구현한 기능에 대한 단위 테스트 진행
- 함수는 최대 15라인
- else 지양하고 return 바로
