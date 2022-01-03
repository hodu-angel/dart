```
List membersList = [
	{
		‘id’ : 0,
		‘group’ : ‘레드벨벳’,
		‘name’ : ‘아이린’
	},
	{
		‘id’ : 1,
		‘group’ : ‘BTS’,
		‘name’ : ‘RM’
	},
	{
		‘id’ : 2,
		‘group’ : ‘레드벨벳’
		‘name’ : ‘슬기’,
	}
];
```
- list.forEach
```
memebersList.forEach((item){
  print(item);  
});
```
<br>

- list의 일부 요소 list출력
```
var nameList = membersList.map((item){
 return item['name'];   
});
print(nameList);
```
<br>

- fold
-loop이 매번 돌때마다 0부터 시작하여 t(total)에 element의 요소를 계속 더한다.
```
var fold = memebersList.fold(0, (t, e){
    return t + e['id'];     
});
print(fold);    //3
```
<br>

- reduce
```
var reduce = [1,2,3,4,5].reduce((t, i)=> t+i);
print(reduce);  //15
```
<br>

### **fold와 reduce 차이**
> fold는 반환값이 어느것이 되던 상관이 없지만, reduce는 t, i의 변수 타입이 같아야 된다.