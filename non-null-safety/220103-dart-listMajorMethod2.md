## List 주요 method
```
List numbersList = [10, 20, 30, 40, 50];
```
<br>

- 값을 알고 있을 때 제거
```
numbersList.remove(10);
print(numbersList);     //[20, 30, 40, 50]
```
<br>

- index로 제거
```
numbersList.removeAt(1);
print(numbersList);     //[20, 40, 50]
```
<br>

- 조건에 맞는 것 제거
```
numbersList.removeWhere( (e) => e ==50 );
print(numbersList);     //[20, 40]
```
<br>

- 섞기
```
numbersList.shuffle();
print(numbersList);
```