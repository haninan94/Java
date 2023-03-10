# 연산자

## 기본 연산자

> **항과 연산자**

- 단항 연산자

항이 한개인 연산자 입니다. ++num 과 같이 사용합니다.

- 이항 연산자

항이 두개인 연산자 입니다. 일반적인 사칙연산이 이항 연산자에 해당됩니다.

- 삼항 연산자

항이 세개인 연산자 입니다. (2 > 4) ? 1 : 0; 와 같이 사용할 수 있습니다.

> **대입 연산자**

대입 연산자는 변수에 값을 대입하는 연산자 입니다. 오른쪽 변수 값이나 식의 연산 결과 값을 왼쪽 변수에 대입합니다.

> **산술 연산자**

- +

두 항을 더합니다.

- -

앞쪽의 항에서 뒤에 있는 항을 뺍니다.

- *

두 항을 곱합니다.

- /

앞에 있는 항에서 뒤에 있는 항을 나누어 몫을 구합니다.

- %

앞에 있는 항에서 뒤에 있는 항을 나누어 나머지를 구합니다.

- 산술연산자 우선순위는 일반적인 사칙연산자의 우선수위와 동일합니다.

> **증가, 감소 연산자**

```java
val = ++num; // 먼저 num의 값이 1 증가한 후 val에 대입합니다.
val = num++; // 먼저 num의 값이 val에 대입되고 num값이 1 증가합니다.
val = --num; // 먼저 num의 값이 1 감소한 후 val에 대입합니다.
val = num--; // 먼저 num의 값이 val에 대입되고 num값이 1 감소합니다.
```

> **관계 연산자**

|연산자|기능|연산 예|
|---|---|---|
|>|왼쪽 항이 크면 참을, 아니면 거짓을 반환합니다.|num > 3;|
|<|왼쪽 항이 작으면 참, 아니면 거짓을 반환합니다.|num < 3;|
|>=|왼쪽 항이 오른쪽 항보다 크거나 같으면 참, 아니면 거짓을 반환합니다.|num>= 3;|
|<=|왼쪽 항이 오른쪽 항보다 작거나 같으면 참, 아니면 거짓을 반환합니다.|num<=3;|
|==|두 개 항의 값이 같으면 참, 아니면 거짓을 반환합니다.| num== 3;|
|!=|두 개의 항이 다르면 참, 아니면 거짓을 반환합니다.|num != 3;|

> **논리 연산자**

논리 연산자는 명제를 생각하면 됩니다. 두 명제가 모두 참이면 논리의 곱은 참이고, 두 명제 중 하나만 참이면 논리 합은 참입니다. 참의 부정은 거짓, 거짓의 부정은 참입니다.

|연산자|기능|연산 예|
|---|---|---|
|&&(논리 곱)|두 항이 모두 참인 경우에만 결과 값이 참입니다. 그렇지 않은 경우는 거짓입니다.|boolean val = (5 > 3) && (5 > 2);|
| ㅣㅣ(논리 합)|두 항 중 하나의 항만 참이면 결과 값은 참입니다. 두 항이 모두 거짓이면 결과 값은 거짓입니다.|boolean val = (5 > 3) || (5 < 2);|
|!(부정)|단항 연산자입니다. 참인 경우는 거짓으로 바꾸고, 거짓인 경우는 참으로 바꿉니다.|boolean val = !( 5> 3);|

> **조건 연산자**

조건 연산자는 연산에 필요한 항의 개수가 세 개입니다. (삼항 연산자)

|연산자|기능|연산 예|
|---|---|---|
|조건식 ? 결과1 : 결과2;|조건식이 참이면 결과1, 조건식이 거짓이면 결과2가 선택됩니다.|int num = (5 > 3) ? 10 : 20;|

## 비트 연산자

> **비트 논리 연산자**

비트 단위로 &, |, ^, ~ 연산이 이루어집니다.

- &(AND) 연산자는 두 개의 비트 값이 모두 1인 경우에만 연산의 결과 값이 1이 됩니다.

- |(OR) 연산자는 비트 값이 하나라도 1이며 연산 결과 값이 1이 됩니다.

- ^(XOR) 연산자는 같으면 0, 다른 값이면 1의 결과값을 같습니다.

- ~(반전) 연산자는 비트 값을 0은 1로, 1은 0으로 바꾸는 연산자입니다.

> **비트 이동 연산자**

- << 연산자

<< 시프트 연산자는 왼쪽으로 비트를 이동하는 연산자 입니다.

- \>> 연산자

\>> 시프트 연산자는 오른쪽으로 비트를 이동하는 연산자 입니다.

- \>>> 연산자

\>>> 시프트 연산자는 \>> 연산과 동일하게 비트를 오른쪽으로 이동합니다. 차이가 있따면 왼쪽에 채워지는 비트 값이 부호 비트와 상관없이 무조건 0이 됩니다.

> **연산자 우선순위**

- 단항 연산자가 가장 높고 이항,삼항 연산자 순서입니다.

- 대입 연산자의 우선순위가 가장 낮습니다.

- 산술, 관계, 논리, 대입 연산자 순서로 우선수위를 가지며 ( )의 우선순위가 가장 높습니다.
