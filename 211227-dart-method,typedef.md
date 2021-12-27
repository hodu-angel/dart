- **함수**
-dart는 오버로딩이 되지 않는다.
```
void main(){
    double answer = linearEx(1,2,3);
    print(answer);  //5
    double answer2 = linearEx2(1,2);
    print(answer2); //4
    double answer3 = linearEx3(1,2, b:10);
    print(answer3);  //12
    double answer4 = linearEx3(1,2);
    print(answer4);
}
//ax+b
double linearEx(double a, double b, double x){
    return a*x+b;
}
```
<br>

- **b를 옵션으로 주기**
-default 값을 줘야 된다.
-a,x는 positional Parameter 라고 한다. 어떤 위치에 어떤 값을 넣는지 정하기 때문이다.
```
double linearEx2(double a, double x, [double b =2]){
    return a*x+b;
}
```
<br>

- **named Parameter**
```
double linearEx3(double a, double x, {
    double b
}){ return a*x+b; }
```
<br>

<hr>

- **typedef**
-함수 시그니처를 저장하고 변수처럼 사용할 수 있는 방법
```
void main(){
    calculate(1,2,add); //3
}
typedef Operation(int x, int y);
void add(int x, int y){
    print('결과값 : ${x+y}');
}
void substract(int x, int y){
    print('결과값 : ${x-y}');
}
void calculate(int x, int y, Operation oper){
    oper(x,y);
}
```