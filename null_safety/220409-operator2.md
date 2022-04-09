# operator2
- 비교연산
```
void main(){
    int num = 1;
    int num2 = 2;
    
    print(num > num2);  //false
    
    print(num < num2);  //true
    
    print(num >= num2); //false
    
    print(num <= num2); //true
    
    print(num = num2);  //false
    
    print(num != num2)  //true
}
```

<br><br>

- type을 비교하는 operator
> 변수 is type : 변수타입이 type과 일치하면 true<br>
> 변수 is! type : 변수타입이 type과 일치하지 않으면 true <br>
```
void main(){
    int num = 1;
    
    print(num is int);  //true
    
    print(num is String);   //false
    
    print(num is! int)  //false
    
    print(num is! String)   //true
}
```