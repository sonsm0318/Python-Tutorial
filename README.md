## 학습 내용

### 파이썬

---

Python은 귀도 반 로섬이 창작하여 1991년에 출시된 언어로 웹 개발 및 소프트웨어 개발에 사용된다. 파이썬의 장점은 영어와 유사한 구문으로 쉽게 배울 수 있으며 다양한 플랫폼들에서 작동할 수 있다.

### 시작하기

---

Linux의 경우 명령줄 Mac의 경우 터미널을 열어 python 혹은 py를 입력할 경우 파이썬을 실행할 수 있다.

파이썬 혹은 다른 프로그래밍 언어를 처음 배울 때 ‘Hello World’를 출력하는 것으로 주로 시작하며 파이썬의 출력 명령어는 print(”원하는 문구”) 를 사용할 수 있다

파이썬을 종료하고 싶을 때는 exit() 명령어를 통해 종료할 수 있다

### 주석

---

파이썬은 # 기능을 통해 주석을 달 수 있다. 만약 여러 줄을 동시에 주석 처리하고 싶을 때는 “””을 시작으로 “””로 끝내면 문자열로 인식하여 주석처럼 사용이 가능하다.

"""

This is a comment

written in

more than just one line

"""

#코멘트

print("Hello, World!")

### 변수

---

변수를 지정할때 숫자는 그냥 써도 되지만 문자의 경우 “”를 붙여야한다.

파이썬은 “와 ‘를 구분하지 않아 혼용해서 사용해도 좋다.

변수 이름은 처음에 숫자가 올 수 없으며, 공백 사용이 불가하고, 특수 문자가 올 수 없다.

변수는 함수 내에서 지정하게 될 경우 지역 변수가 되며 이를 방지하고 싶을때 함수 밖에서 변수를 지정하거나 global 명령어를 사용할 수 있다.

x = ”awesome"

def myfunc():

  x = "fantastic"

  print( x)

myfunc()

print( x)

위의  식을 출력하게 되면 awesomefantastic가 출력된다.

### 문자 유형

---

| 텍스트 유형: | str |
| --- | --- |
| 숫자 형식: | int,float,complex |
| 시퀀스 유형: | list,tupe,range |
| 매핑 유형: | dict |
| 세트 유형: | set,frozenset |
| 부울 유형: | bool |
| 바이너리 유형: | bytes,bytearray,memoryview |
| 없음 유형: | NoneType |

문자 유형은 해당 유형을 입력할 경우 자동으로 입력되고 만약 직접 지정하고 싶을때는 위의 문법을 사용하면 직접 유형이 지정된다.

### 숫자

---

숫자 유형에는 int,float,complex가 있으며 각각 정수, 유리수, 복소수를 의미한다.

x = 3   

y = 2.3  

z = 1+4j

위의 식을 입력하면 x는 int ,y는 float, z는 complex 타입으로 지정이 되며, 

n=complex(x)

위의 식을 입력하게 되면 타입은 복소수에 값이 3으로 지정된다.

### 문자열

---

문자열은 “”를 통해 입력할 수 있으며 만약 여러줄에 나눠 입력하고 싶을때는 “””를 시작과 끝에 붙혀 문자열을 입력할 수 있다. 문자열에 사용할 수 있는 명령어는 아래와 같다.

| a[x] | a 문자열의 x위치의 문자를 출력 |
| --- | --- |
| len(a) | a 문자열의 길이를 반환 |
| in | 문자열 안에 해당 문자가 있는지 확인 |
| a[x:y] | a 문자열의 위치 x부터 y까지 가져오기(x 포함 y 비포함) |
| a.upper() | a 문자열을 대문자로 변환 |
| a.lower() | a 문자열을 소문자로 변환 |
| a.strip() | a 문자열의 양 끝 공백 제거 |
| a.replace(”x” , “y”) | a 문자열의 x 문자를 y 문자로 변환 |
| a.split(”x”) | a 문자열을 x를 기준으로 나워 하위 문자열로 분할 |
| a+b | a 문자열과 b 문자열을 병합 |
| a.format(x) | a 문자열의 {}를 숫자 x 로 변환 |

위의 명령어 외에도 많은 메소드가 존재하며 만약 문자열에 특수 문자를 쓸때 버그가 발생하는데 이런 것들을 위해 이스케이프 문자를 쓸 수 있다.

| \' | Single Quote | ‘ 출력 |
| --- | --- | --- |
| \\ | Backslash | / 출력 |
| \n | New Line | 줄 바꾸기 |
| \r | Carriage Return | 맨 앞줄 이동 |
| \t | Tab | 탭 |
| \b | Backspace | 지우기 |
| \f | Form Feed |  |
| \ooo | Octal value | 8 진수  |
| \xhh | Hex value | 16 진수 |

### 참 거짓

---

bool() 함수는 해당 값의 참 거짓을 판별하는 함수로, 0이 아닌 모든 값을 참으로 표기하게 된다. 따라서 비교 연산자를 사용하는게 아닌 상황에서 False와 0을 입력하는게 아니라면 모든 값을 True로 출력하게 되어있다.

a = 1==2

b = “face”

c = 0

위의 값을 입력하게 되면 b를 제외하고 a,c 모두 False가 출력된다.

### 연산자

---

산술 연산자

| + | 더하기 | x + y |
| --- | --- | --- |
| - | 빼기 | x - y |
| * | 곱하기 | x * y |
| / | 나누기 | x / y |
| % | 나머지 | x % y |
| ** | 제곱 | x ** y |
| // | 정수 나누기 | x // y |

할당 연산자

| = | 값 할당 | x = 5 |
| --- | --- | --- |
| += | 기존 값에 값을 더하여 할당 | x = x + 3 |
| -= | 기존 값에 값을 빼서 할당 | x = x - 3 |
| *= | 기존 값에 값을 곱하여 할당 | x = x * 3 |
| /= | 기존 값에 값을 나누어 할당 | x = x / 3 |
| %= | 기존 값에 값을 나눈 나머지 값 할당 | x = x % 3 |
| //= | 기존 값에 값을 나눈 값의 가장 가까운 정수 할당 | x = x // 3 |
| **= | 기존 값에 제곱을 할당 | x = x ** 3 |
| &= | 비트 연산 and | x = x & 3 |
| |= | 비트 연산 or | x = x | 3 |
| ^= | 비트 연산 xor | x = x ^ 3 |
| >>= | a 비트를 b번 오른쪽 이동 후 할당 | x = x >> 3 |
| <<= | a 비트를 b번 왼쪽 이동 후 할당 | x = x << 3 |

비교 연산자

| == | 같다 | x == y |
| --- | --- | --- |
| != | 같지 않다 | x != y |
| > | 크다 | x > y |
| < | 작다 | x < y |
| >= | 크거나 같다 | x >= y |
| <= | 작거나 같다 | x <= y |

논리 연산자

| and | 두 값 모두 | x < 5 and  x < 10 |
| --- | --- | --- |
| or | 두 값 중 하나라도 | x < 5 or x < 4 |
| not | 아닌 | not(x < 5 and x < 10) |

이 외

| is | Returns True if both variables are the same object | x is y |
| --- | --- | --- |
| is not | Returns True if both variables are not the same object | x is not y |
| in  | Returns True if a sequence with the specified value is present in the object | x in y |
| not in | Returns True if a sequence with the specified value is not present in the object | x not in y |
| &  | AND | Sets each bit to 1 if both bits are 1 |
| | | OR | Sets each bit to 1 if one of two bits is 1 |
| ^ | XOR | Sets each bit to 1 if only one of two bits is 1 |
| ~ | NOT | Inverts all the bits |
| << | Zero fill left shift | Shift left by pushing zeros in from the right and let the leftmost bits fall off |
| >> | Signed right shift | Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off |

### 목록,튜플,세트

---

목록,튜플,세트는 각각 (),[],{}를 통해 나타내며 여러 값을 한 곳에 넣을 수 있다. 세개 모두 len과 in 명령어가 사용가능하며 각각의 특징으로는 튜플은 변경이 불가하고 세트의 경우 집합연산이 가능하다. 

| 목록 | 세트 | 기능 |
| --- | --- | --- |
| append() | add() | 항목 추가 |
| extend() | update() | 다른 목록, 세트를 추가 |
| insert() |  | 특정 인덱스 삽입 |
| remove() | remove(),discard() | 지정 값 삭제, remove는 값이 없을때 에러가 뜨며 disard는 뜨지 않는다 |
| pop() | pop() | 지정 값 삭제 밑 반환 |
| clear() | clear() | 모든 항목 제거 |

### 딕셔너리

---

값을 쌍으로 저장할 수 있는 데이터 유형

passport = {

  "country": "KOREA",

  "name": "SAM",

  "birth”: 1964

}

위와 같이 딕셔너리를 지정할 수 있다.

| keys(), values(), items() | 모든 키, 값, 키-값 을 변환한다. |
| --- | --- |
| dict[’’] = ‘’ | 키-값 추가 |
| del dict[’’] | 키값 제거 |
| get() | 키 값 반환 |
| clear | 모든 키 값 제거 |
| pop() | 지정 값 삭제 밑 반환 |
| update() | 다른 딕셔너리를 추가 |

### if문

---

if문은 뒤의 문장이 옳으면 아래의 문장을 출력하고 틀리면 else 뒤의 문장을 출력한다. elif를 사용하면 2개 이상의 판단문을 사용할 수 있다.

a=20

if a<5:

  print(1)

elif 5≤x<10:

  print(2)

else:

  print(3)

위의 문장을 출력할 경우 3이 나오게 된다.

### while,for문

---

while은 뒤의 문장이 참일 경우 계속해서 아래의 문장을 출력하고 for문의 경우 뒤의 값을 0부터 차례로 출력한다. 만약 이 반복문들을 깨고 싶을때는 break를 사용할 수 있다.
