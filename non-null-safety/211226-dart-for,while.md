- **for**
```
dynamic total = 0;
List numbersList = [1,1,2,3,5,8];
for(int i = 0; i<numbersList.length; i++){
    total += numbersList[i];
}
print(total);
```
<br>

- **for in**
```
for(int number in numbersList){
    total += number;
}
print(total);
```
<br>

- **while**
```
int total = 0;
while(total < 10){
    total++;
}
print(total);   //10
```
<br>

- **do-while**
```
int total = 0;
do{
    print(total);   //0~19출력
    total++;
}while(total < 20);
```