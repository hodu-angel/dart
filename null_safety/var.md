# var

- 변수 선언
> 변수앞엔 숫자사용이 불가하다. 
> '_'는 사용 가능
```
void main(){
    var name = 'hodu';
    print(name);
    
    var name2 = 'angel';
    print(name2);
    
    var 1name = 'hodu'; //compile error
    print(1name);
}
```

<br>

- 값 변경
```
void main(){
    var name = 'hodu';
    name = 'hodu2';
    print(name);    //hodu2
}
```

<br>

- 동일한 변수명 사용 불가
```
void main(){
    var name = 'hodu';
    var name = 'angel'; //compile error
}
```