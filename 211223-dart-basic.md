- **출력**
파이썬과 유사하다.
print('hi');

---
- **변수 초기화**
-처음 지정될떄의 데이터타입으로 결정된다. 이후에 다른 데이터타입이면 오류난다.
-처음에 초기화 하지 않고 선언만 해두면 dynamic처럼 사용가능하다.
1.
```
var name = 'dart 언어';
//변경
name = '강좌시작';
```
<br>

2.
```
var name;
name = 'dart 언어';
name = 1;   //error 안 남
```
<br>

---
- **숫자타입 2가지**
1. int
```
int number1 = 12;
print(number1);
```
<br>

2. double
```
double number2 = 20.0;
print(number2);
```
<br>

---
- **String**
1. '+' 연산자를 이용한 문자열 출력
```
String name = '효주';
String group = '취준생';
print(name + '는' + group);
```
<br>

2. 문자열 안에 변수 넣기
```
print('$name는 $group입니다.')
```
<br>

3. 복잡한 코드 작성
```
print('${name + '는' + group} 입니다.');
```
<br>

---
- **true false**
```
bool isTrue = true;
bool isFalse = false;
print(isTrue);
print(isFalse);
```
<br>

---
- **dynamic**
-기존 var 로 인해 후에 데이터타입 변경시 오류가 발생했던 문제를 해결하기 위해 dynamic가 등장하였다.
```
dynamic name = '효주';
print(name);
name = 1;
print(name);    //error 안남
```