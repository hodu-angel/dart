## break문
- loop를 탈출한다.

1. 일반적인 loop에서의 break문
```
void main(){
    int tot = 0;
    
    while(tot < 10){
        tot += 1;
        
        if(tot == 5){
            break;
        }
    }
    print(tot); //5
}
```
<br><br>

2. for_loop에서의 break문
```
void main(){
    int tot = 0;
    
    for(int i = 0; i < 10; i++){
        tot += 1;
        
        if(tot == 5){
            break;
        }
    }
    print(tot); //5
}
```

<br><br><br>

## continue
- for_loop에서 자주 쓰인다.
- 이후의 코드를 실행하지 않고, 조건으로 되돌아 간다.
```
void main(){
    for(int i = 0; i < 10; i++){
        if(i == 5){
            continue;
        }
        print(i);
        //0
        //1
        //2
        //3
        //4
        //6
        //7
        //8
        //9
    }
}
```