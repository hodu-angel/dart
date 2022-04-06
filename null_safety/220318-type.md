# Type
1. 정수(Integer)
```
int number1 = 2;
int number2 = 4;

print(number1 + number2);   //6
print(number1 - number2);   //-2
print(number1 / number2);   //0.5
print(number1 * number2);   //8
```
<br><br>

2. 실수(double)
```
double d_number1 = 2.5;
double d_number2 = 0.5;

print(d_number1 + d_number2);   //3
print(d_number1 - d_number2);   //2
print(d_number1 / d_number2);   //5
print(d_number1 * d_number2);   //1.25
```
<br><br>

3. boolean
```
bool isTrue = true;
bool isFalse = false;

print(isTrue);  //true
print(isFalse); //false
```
<br><br>

4. 문자타입(String)
> String 타입은 덧셈연산만 가능하다.
```
String name = 'hodu';
String name2 = 'angel';

print(name);    //hodu
print(name2);   //angel
print(name + name2);    //hoduangel
print(name + ' ' + name2);  //hdou angel
```

<br>

---

<br>

- var와 String 차이
> var는 오른쪽값으로 유추를 한다.
```
var name3 = 10;
print(name3.runtimeType);   //int
```
<br>

- 변수를 1개이상 사용할땐 ${변수}로 사용한다.
```
String name = 'hodu';
String name2 = 'angel';
print(${name} ${name2});
```
<br>

- 단일 변수를 사용한다면 $변수만 넣어도 된다.
```
print($name $name2);
```
