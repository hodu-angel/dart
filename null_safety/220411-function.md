## function
- 함수는 반복되는 코드를 재활용할 수 있게 선언하는 것이다.
- main은 가장 먼저 실행되는 함수이다.
- 함수의 역할을 comment해주는 것이 좋다.
- parameter만 변경해서 로직 그대로를 사용할 수 있다.

<br>

- void
> 공허, 아무것도 없다는 의미이다. <br>
> return type이다. <br>

<br>

---

<br>

1. 기본적인 함수
```
void main(){
    speak();    //speak function
}

speak(){
    print('speak function');
}
```
<br><br>

2. positional parameter
> parameter = argument = 매개변수 <br>
> 순서가 중요한 parameter이다. <br>

```
void main(){
    addNumbers(10,20,30);   //짝수입니다.
}

//세개의 숫자(x, y, z)를 더하고 짝수인지 홀수인지 알려주는 함수.
addNumbers(int x, int y, int z){
    int sum = x + y + z;
    
    if(sum % 2 == 0){
        print('짝수입니다.');
    } else {
        print('홀수입니다.');
    }
}
```
<br><br>

3. optional parameter
> 있어도 되고 없어도 되는 parameter이다. <br>
> [ ]로 표현 <br>
> 기본값을 적어줘야 된다. <br>

```
void main(){
    optionalNumbers(10);    //짝수입니다.
}

optionalNumbers(int x, [int y = 1, int z = 1]){
    int sum = x + y + z;
    
    if(sum % 2 == 0){
        print('짝수입니다.');
    } else {
        print('홀수입니다.');
    }
}
```
<br><br>

4. naemd parameter
> 이름이 있는 parameter이다. <br>
> 순서가 중요하지 않다. <br>
> naemd parameter에서는 optional parameter를 사용할 수 있다. <br>
> 호출: 함수명(변수1: 값1, 변수2: 값2 ...) <br>

```
void main(){
    namedNumbers(x:10, y:20);   //짝수입니다.
}

namedNumbers({
    required int x,
    required int y,
    int z = 30,
}){
    int sum = x + y + z;
    
    if(sum % 2 == 0){
        print('홀수입니다.');
    } else {
        print('짝수입니다.');
    }
}
```
<br><br>

5. arrow function(화살표 함수)
```
void main(){
    int result = addNumbers(10, 20);
    print(result);  //30
}

int addNumbers(int x, int y) => x + y;
```