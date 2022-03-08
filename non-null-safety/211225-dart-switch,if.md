- **switch-case**
```
enum Status{
    approved,
    rejected,
    pending,
}
void main(){
    Status status = Status.approved;
    switch(status){
        case Status.approved:
            print('승인 상태');
            break;
        case Status.rejected:
            print('거절 상태');
            break;
        case Status.pending:
            print('대기 상태');
            break;
        default:
            print('어디에도 해당되지 않습니다.');
            break;
    }
}
```
<br>

- **if**
```
int number = 3;
if(number % 3 == 0){
    print('3의 배수입니다.');
} else if(number % 2 == 0){
    print('2의 배수입니다.');
} else {
    print('어떤 배수인지 알 수 없습니다.');
}
```
<br>

위 코드를 switch-case문으로 작성한다면.
```
switch(number % 3){
    case 0:
        print('3의 배수입니다.');
        break;
    case 2:
        print('2의 배수입니다.');
        break;
    default:
        print('어떤 배수인지 알 수 없습니다.');
        break;
}
```