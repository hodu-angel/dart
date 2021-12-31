- **List주요 method**
```
List redVelvet = [
    '아이린',
    '슬기',
    '웬디',
    '조이',
    '예리',
];
```
---

- 첫번째 요소 출력
```
print(redVelvet.first); //아이린
```
<br>

- 비어있는지 확인
```
print(redVelvet.isEmpty);   //false
```
<br>

- 안 비어있는지 확인
```
print(redVelvet.isNotEmpty);    //true
```
<br>

- 길이 구하기
```
print(redVelvet.length);    //5
```
<br>

- 마지막 요소 출력
```
print(redVelvet.last);  //예리
```
<br>

- 요소 거꾸로 출력
```
print(redVelvet.reversed);  //(예리, 조이, 웬디, 슬기, 아이린)
```
<br>

- 리스트에 추가하기
```
redVelvet.add('hyo');
print(redVelvet);   //[아이린, 슬기, 웬디, 조이, 예리, hyo]
```
<br>

- 한번에 리스트에 추가하기
```
redVelvet.addAll(['jin', 'army']);
print(redVelvet);    //[아이린, 슬기, 웬디, 조이, 예리, hyo, jin, army]
```