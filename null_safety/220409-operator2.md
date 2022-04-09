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

<br><br>

- 논리 operator
> a && b 연산자 : a 와 b둘다 true이면 true <br>
> a || b 연산자 : a 또는 b 둘 중 하나가 true이면 true <br>
```
void main(){
    bool result = 12 > 10;  //true
    
    bool result2 = 12 > 10 && 1 > 0;
    print(result2); //true
    
    bool result3 = 12 > 10 && 0 > 1;
    print(result3); //false
    
    bool result4 = 12 > 10 || 1 > 0;
    print(result4); //true
    
    //둘중 하나라도 true이면 true
    bool result5 = 12 > 10 || 0 > 1;
    print(result5); //true
    
    bool result6 = 12 < 10 || 0 > 1;
    print(result6); //false
}
```