# 로또 발매기 프로그램

## 프로젝트 개요
- **간단한 로또 발매기 구현한다.** 
- **관련 함수를 묶어 클래스를 만들고, 객체들이 협력하여 하나의 큰 기능을 수행하도록한다.**
- **클래스와 함수에 대한 단위 테스트를 통해 의도한 대로 정확하게 작동하는 영역을 확보한다.**

## 주요 기능
- **로또 구입 금액 입력**: 사용자가 로또 구매를 위한 금액을 입력한다. 로또 한 장의 가격은 1,000원이다. 금액에 해당하는 만큼 로또를 발행한다.
- **로또 번호 생성**: 로또 번호는 1부터 45 사이의 중복되지 않는 숫자 6개로 구성되며, 오름차순으로 정렬한다.
- **구입한 로또 번호 출력**: 구매한 로또의 개수와 번호를 출력합니다.
- **당첨 번호 및 보너스 번호 입력**: 사용자가 당첨 번호와 보너스 번호를 입력한다.
- **당첨 내역 계산**: 구매한 로또 번호와 당첨 번호를 비교하여 1등부터 5등까지의 당첨 내역을 출력한다.
- **수익률 계산**: 전체 수익률을 계산하고 소수점 둘째 자리에서 반올림하여 출력한다.
- **예외 처리**: 입력값이 올바르지 않을 경우 `[ERROR]`로 시작하는 메시지를 출력하고 다시 입력을 받습니다.

## 기능 목록
1. **로또 구입 금액 입력 처리**
   - 사용자 입력값이 1,000원 단위인지 검증.
   - 예외 처리: 1,000원 단위로 나누어떨어지지 않으면 예외 발생.

2. **로또 번호 생성 및 출력**
   - 1에서 45 사이의 중복되지 않는 6개의 숫자를 생성하여 오름차순으로 정렬.

3. **구입한 로또 번호 출력**
   - 사용자에게 구매한 로또의 개수와 번호를 출력.

4. **당첨 번호 입력 처리**
   - 당첨 번호는 쉼표(,)로 구분된 6개의 숫자.
   - 예외 처리: 중복 숫자, 숫자 범위 외 입력 등.

5. **보너스 번호 입력 처리**
   - 사용자로부터 보너스 번호 입력.
   - 예외 처리: 중복 여부 및 숫자 범위 검증.

6. **당첨 내역 계산 및 출력**
   - 로또 당첨 내역을 계산하고 각 등수의 당첨 개수 출력.
   - 3개 일치(5,000원), 4개 일치(50,000원), 5개 일치(1,500,000원), 5개 + 보너스 번호 일치(30,000,000원), 6개 일치(2,000,000,000원).

7. **수익률 계산**
   - 총 당첨 금액을 구입 금액 대비 비율로 계산하여 출력.
   - 소수점 둘째 자리에서 반올림.

8. **예외 처리**
   - 잘못된 입력값 처리 및 `[ERROR]` 메시지 출력 후 재입력 유도.
   - Exception이 아닌 IllegalArgumentException, IllegalStateException 등과 같은 명확한 유형을 처리.

