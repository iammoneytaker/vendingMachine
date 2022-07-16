# vendingMachine
책 '디자인 씽킹을 넘어 프로그래밍 씽킹으로'를 보고 자판기의 알고리즘을 생각하게 되었고 이것을 바탕으로 웹 상에서 자판기를 구현해보려고 합니다.

## 첫 번째 생각
1. 손님이 자판기에 돈을 넣는다.
2. 음료를 선택한다.
3. 음료가 나온다.
4. 거스름 돈을 반환한다.

## 다각도로 접근한 생각
1. 손님이 자판기에 돈을 넣을 때 100원, 500원, 1000원, 5000원 인지 확인한다.
2. 넣은 돈이 700원이상이면 오렌지 주스, 사과 주스, 물, 매실 주스 의 버튼이 활성화 된다.
3. 넣은 돈이 1000원이상이면 포카리스웨트의 버튼이 활성화 된다.
4. 넣은 돈이 1300원이상이면 콜라,사이다,마운틴듀의 버튼이 활성화 된다.
5. 손님이 활성화된 버튼을 누르면 음료를 내보낸다.
6. 거스름돈을 반환한다.

## 깊게 생각하기
- 깊게 생각하기

(돈을 넣었을 때)
손님이 자판기에 돈을 넣을 때 동전인지 지폐인지 구분한다.
만약 자판기에 넣은 돈이 동전이라면 100원, 500원이 아니라면 다시 반환한다.
만약 자판기에 넣은 돈이 지폐라면 1000원권 5000원권이 아니라면 다시 반환한다.

(자판기의 잔돈 여부 파악 및 음료들의 활성화 여부)
넣은 돈이 700원 이상일 때 자판기에 잔돈을 확인한 후 잔돈이 있다면 700원 대의 음료들의 개수를 파악하고 1개 이상이 있는 음료들의 버튼을 활성화 한다.
만약 잔돈이 없다면 잔돈 없음 표시를 하고 다시 넣은 돈을 반환한다.음료가 없다면 해당 음료의 버튼에는 재고 부족이라고 나타낸다.

넣은 돈이 1000원 이상일 때 자판기에 잔돈을 확인한 후 잔돈이 있다면 1000원 대의 음료들의 개수를 파악하고 1개 이상이 있는 음료들의 버튼을 활성화 한다.
만약 잔돈이 없다면 잔돈 없음 표시를 하고 다시 넣은 돈을 반환한다.음료가 없다면 해당 음료의 버튼에는 재고 부족이라고 나타낸다.

넣은 돈이 1300원 이상일 때 자판기에 잔돈을 확읺한 후 잔돈이 있다면 1000원 대의 음료들의 개수를 파악하고 1개 이상이 있는 음료들의 버튼을 활성화 한다.
만약 잔돈이 없다면 잔돈 없음 표시를 하고 다시 넣은 돈을 반환한다. 음료가 없다면 해당 음료의 버튼에는 재고 부족이라고 나타낸다.

( 음료를 선택했을 때)
손님이 활성화 된 버튼을 누르면 음료를 내보낸다.
모든 음료의 버튼을 비활성화 처리한다. 
손님이 넣은 돈에서 누른 버튼의 음료 가격만큼 차감을 하고
해당 가격에서 선택할 수 있는 음료들의 개수를 파악하고 버튼을 활성화 시킨다. 

(잔돈 반환을 눌렀을 때)
손님이 잔돈 반환 버튼을 누르면 잔돈을 반환한다.


(관리자)
비밀번호를 통해서 자판기의 문을 열 수 있다.

자판기의 문이 열리면 음료들의 개수를 파악할 수 있다.
자판기의 문이 열리면 잔돈의 여부를 파악할 수 있다.

잔돈을 채울 수 있다.
음료를 채울 수 있다.
