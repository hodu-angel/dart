- **final**
-변수의 값을 바꿀 수 없다.
```
final lang = '자바';
final String lang2 = 'c';
lang = '파이썬' //error
```
<br>

- **const**
변수의 값을 바꿀 수 없다.
```
const lang3 = '파이썬';
const String lang4 = 'dart';
```
<br>

- final과 const의 차이
>final은 runTime에서 변경되지 않는 선에서 값이 지정되어도 상관없다.
const는 buildTime에 꼭 값이 지정되어 있어야 된다.
>
>쉽게 말하자면, 
>const는 실행시에 결정되는 값을 설정할 수 없다. 정해진 값만 가능하다.
>final은 실행시에 결정되는 값도 설정할 수 있다.

<br>

- 현재 시각 받아오기
```
final now = new DateTime.now();
print(now);
```