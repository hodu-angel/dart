# operator
- 기본적인 사칙연산
```
void main(){
    double num = 4.0;
    print(num); //4
    
    num += 1;
    print(num); //5
    
    num -= 1;
    print(num); //4
    
    num *= 2;
    print(num); //8
    
    num /= 2;
    print(num); //4
}
```
<br><br>

- null일 때 대입
> ??= 연산자 사용
```
void main(){
    double? num = 4.0;
    
    num = null;
    print(num); //null
    
    null ??= 3.0;
    print(num)  //3
}
```