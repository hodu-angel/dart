# null-safety
> nullable: null이 될 수있다. <br>
> non-nullable: null이 될 수 있다. <br>
> null: 아무런 값도 있지 않다. <br>

- ? : null값을 허용한다.
```
String name = null;    //compile error
String? name2 = null;
print(name2);
```
<br><br>

- ! : null이 절대 아니다
```
String? name2 = 'hodu';
print(name2!);
```