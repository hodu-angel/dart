- **List 탐색**
```
List membersList = [
    {
        'id' : 0,
        'name' : '슬기'
    },
    {
        'id' : 1,
        'name' : '아이린'
    },
    {
        'id' : 2,
        'name' : '조이',
    }
];
```
---

- 첫번째로 조건에 해당되는 것을 찾음
```
var item = membersList.firstWhere( (item) => item['id'] == 1 );
```
<br>

- 인덱스 찾기
```
var index = membersList.indexWhere( (item) => item['id'] == 2);
```
<br>

- 같은 것 찾기 (같으면 index반환 다르면 -1반환)
```
var index2 = [10,20,30].indexOf(20);    //1
```
<br>

- 포함 되어 있는지 확인(true or false 반환)
```
var contains = [10,20,30].contains(30); //true
```