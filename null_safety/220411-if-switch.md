## if
- if(조건){ 조건이 true일 경우 실행할 code }
- else if(조건){ 조건이 true일 경우 실행할 code}   //else if에서 조건에 부합하면 이후 조건문을 거치지 않는다.
- else는 모든 if문을 제외한 것이므로 조건을 작성하지않고 { } 만을 사용한다.
```
void main(){
    int num = 2;
    if(num % 3 == 0){
        print('나머지가 0 입니다.');
    } else if(num % 3 == 1){
        print('나머지가 1 입니다.');
    } else {
        print('나머지가 2입니다.');
    }
}
```
<br><br>

## switch
- switch(조건문){ case 값1: break; case 값2: break; default: break;}
```
void main(){
    int num = 3;
    switch(num % 3){
        case 0:
            print('나머지가 0 입니다.');
            break;
        case 1:
            print('나머지가 1 입니다.');
            break;
        default:
            print('나머지가 2입니다,');
            break;
    }
}
```