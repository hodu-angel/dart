- **static**
-인스턴스에 귀속되지 않고, 클래스째로 귀속이 된다.
-static을 사용하면 this를 사용하지 않는다.(사용 자체가 불가하다.)
-Static keyword이기 때문에 클래스에 직접 접근하여 사용한다.

```
class Employee{
    static String building;
    String name;
    
    Employee(
        String name,
    ) : this.name = name;
    
    void printNameAndBuilding(){
        print('이름은 $name이고 건물은 $building입니다.');
    }
    static void printBuilding(){
        print('건물은 $building 입니다.');
    }
}

void main(){
    Employee emp1 = new Employee('사원1');
    Employee emp2 = new Employee('사원2');
    Employee.building = 'dart';
}
```
<hr>

- **Interface**
-상속시 implements 사용
```
//Interface
class IdolInterface{
    void printName(){}
}

class BoyGroup implements IdolInterface{
    ...
    //printName()을 작성하지 않으면 컴파일오류
    void printName(){
        print('제 이름은 ${this.name}입니다.');
    }
}
```
<hr>

- **class method 한번에 호출**
- 기존
```
void main(){
    BoyGroup bts = new BoyGroup('BTS');
    bts.printName();
    bts.printGroup();
}
```
<br>

- 한번에 작성
```
new BoyGroup('BTS')
    ..printName()
    ..printGroup();
    
```