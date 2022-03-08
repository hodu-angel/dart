```
Map price = {
    'iPhone' : 1500000,
    'Galaxy' : 1000000,
    'Apple Watch' : 500000,
};
```
---
<br>

- update
> prev : 이전의 값
> iPhone이라는 키를 찾고 존재하면 값에 10배를 한다.
```
price.update('iPhone', (prev){
    return prev * 10;
});
print(price);
```
<br>

- ifAbsent
> namedParameter인 ifAbsent를 이용해 키가 존재하지 않으면 추가하도록 한다.
```
price.update('Macbook', (prev){
    return prev * 10;
}, ifAbsent: (){
    return 2222;
});
print(price);
```
<br>

- 존재하지 않으면 추가한다.
```
price.putIfAbsent('Macbook Pro', ()=>3333);
print(price);
```
<br>

- all update
```
price.updateAll( (k, v){
    return v.toString() + '원';
});
print(price);
```