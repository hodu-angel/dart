## Map
```
Map price = {
	‘iPhone’ : 1500000,
	‘Galaxy’ : 1000000,
	‘Apple Watch’ : 500000,
};
```
<br>

- 기본 method
```
print(price.isEmpty);       //false
print(price.isNotEmpty);    //true
print(price.keys);          //(iPhone, Galaxy, Apple Watch)
print(price.values);        //(1500000, 1000000, 500000)
print(price.length);        //3
```
<br><br>

### map추가
- 추가 방법1
```
price.addAll({
   'AIrpods' : 390000,
   'Trackpad' : 100000,
});
print(price);
```
<br>

- 추가 방법2
```
price.addEntries([
    MapEntry('Xiaomi', 500000),
    MapEntry('Macbook',2500000),
]);
print(price);
```
<br>

- 추가 방법3
```
price['test'] = 99999;
print(price);
```