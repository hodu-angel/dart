- **List**
1.
```
List btsList = [
    '진',
    '제이홉',
    '뷔',
];
print(btsList);
print(btsList[0]);
print(btsList[2]);
```
<br>

2. 타입을 설정해주면 정확한 데이터의 종류와 개발을 위해서라도 타입을 지정해주는 것이 좋다.
```
List<String> coffee = [
    '라떼',
    '에이드',
    '아아',
];
print(coffee);
print(coffee[0]);
print(coffee[1]);
```
<br>

- 길이출력
```
print(coffee.length);
```
<hr>

- **Map**
1.
```
Map dictionary = {
    'Harry Potter' : '해리포터',
    'Ron Weasley' : '론 위즐리',
};
```
<br>

2. 타입을 설정해주면 정확한 데이터의 종류와 개발을 위해서라도 타입을 지정해주는 것이 좋다.
-key는 절대적으로 유니크 해야된다.
-key가 동일하면 덮어씌워진다.
```
Map<String, String> dictionary2 = {
    'Harry Potter' : '해리포터',
    'Ron Weasley' : '론 위즐리',
};
```
<br>

- 추가하기
```
dictionary2.addAll({
    'Hermione Granger' : '헤르미온느',
});
print(dictionary2);
```
<br>

- 값 변경하기
```
dictionary2['Hermione Granger'] = 'hyo';
print(dictionary2);
```
<br>

- 제거하기
```
//dictionary2.remove(키값);
dictionary2.remove('Hermione Granger');
print(dictionary2);
```
<br>

- key값 출력
```
print(dictionary2.keys.toList());
```
<br>

- value값 출력
```
print(dictionary2.values.toList());
```


