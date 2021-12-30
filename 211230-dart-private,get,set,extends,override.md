- **private**
-변수 앞에 _를 붙여준다.
-다른 폴더에서 접근이 불가하다.
```
class Idol{
    final name;
    final group;
    final _id;  //private
    
    Idol.fromMap(
        Map values
    ) : this.name = values['name'],
        this.group = values['group'],
        this._id = values['id'];
    void printName(){
        print('저는 $group의 $name입니다.');
    }
}
```
<hr>

- **getter setter**
- get
```
get 함수명{
    return;
}
```

또는
get 함수명 => 내용;
<br><br>

- set
```
set 함수명 (매개){
    this.oo = 매개;
}
```
<hr>

- **extends**
```
class GirlGroup extends Idol{
    GirlGroup(
        String name,
        String group,
        int _id,
    ) : super(
        name,
        group,
        _id,
    );
}
```
<br>

- **override**
```
class Parent{
    final int number;
    Parent(
        int number,
    ) : this.number = number;
    int calculate(){
        return this.number * this.number;
    }
}

class Child extends Parent{
    Child(
        int number,
    ) : super(number);
    @override
    int calculate(){
        return this.number + this.number;
    }
}
```