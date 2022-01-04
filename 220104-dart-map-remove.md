### map 제거
```
Map price = {
    'iPhone' : 1500000,
    'Galaxy' : 1000000,
    'Apple Watch' : 500000,
};
```
---
<br>

- 키값으로 제거
```
price.remove('Apple Watch');
print(price);   //{iPhone: 1500000, Galaxy: 1000000}
```
<br>

- 조건으로 제거 (자주 사용됨)
```
price.removeWhere( (k, v){
   return k == 'iPhone'; 
});
print(price);   //{Galaxy: 1000000}
```