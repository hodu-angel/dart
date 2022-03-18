# dynamic
> 기존 var의 타입은 선언할 때의 타입으로 고정이 된다. <br>
> 그래서 중간에 다른 타입으로 변경이 불가능했다. <br>
> dynamic은 중간에 다른 타입으로 변경이 가능하다. <br>
```
dynamic name = 'hodu';
var name2 = 'angel';
print(name.runtimeType);    //String
print(name2.runtimeType);   //String

name = 2;
name2 =5;   //compile error
```