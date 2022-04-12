# typedef
- 함수의 body가 없다.
- typedef의 return type과 parameter type이 같아야 된다.
<br><br>

- 일반적 사용
```
typedef Operation = int Function(
    int x, int y, int z
);

//더하기
int add(int x, int y, int z) => x + y + z;

//빼기
int subtract(int x, int y, int z) => x - y - z;

void main(){
    Operation operation = add;
    int add_result = operation(10, 20, 30);
    print(add_result);  //60
    
    operation = subtract;
    int subtract_result = operation(30, 20, 10);
    print(subtarct_result); //0
}
```
<br>

---

<br>

- 자주 사용되는 방법
```
typedef Operation = int Function(
    int x, int y, int z
);

int add(int x, int y, int z) => x + y + z;

int calculate(int x, int y, int z, Operation operation){ return operation(x, y, z); }
void main(){
    int result = calculate(10, 20, 30, add);
    print(result);  //60
}
```