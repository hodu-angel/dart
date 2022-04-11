## while_loop
> while(조건){ }
```
void main(){
    int tot = 0;
    
    while(tot < 10){
        tot += 1;
    }
    print(tot); //10
}
```
<br><br><br>

## do-while_loop
> do{ 실행코드 } while(조건);
```
void main(){
    int tot = 0;
    
    do{
        tot += 1;
    } while(tot < 10);
    print(tot); //10
}
```
<br><br>

### while와 do-while의 차이
> while은 조건을 먼저 확인하고 조건에 부합하면 코드를 실행한다. <br>

> 그러나 do-while은 코드를 먼저 실행한 후 조건문을 확인한다.
