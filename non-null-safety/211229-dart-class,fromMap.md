- **class**
```
void main(){
    People people = new People(15);
    people.printName();
}
class People{
    String name = 'hyoju';
    final age;
    People(
        int age,
    ) : this.age = age;
    void printName(){
        print('저는 ${this.name} 입니다.');
    }
}
```
<br>

- **fromMap**
```
void main(){
    Idol idol = new Idol.fromMap({
        'name' : '슬기',
        'group' : '레드벨벳',
        });
    idol.printName();
}
class Idol{
    final name;
    final group;
    Idol.fromMap(
        Map values,
    ) : this.name = valuesp['name'], this.group = values['group'];
    void printName(){
        print('저는 $group의 $name 입니다.');
    }
}
```