# final vs const
- 공통점
> 값의 변경이 불가하다. <br>
> var 타입을 생략 할 수 있다. <br>
```
final name = 'hodu';
const name2= 'angel';
```
<br>

---

<br>

### buildTime
> run을 하게 되면 사람의 언어로 작성된 코드를 <br> 
컴퓨터가 이해 할 수 있는 코드인 0101..등으로 변경한다. <br>
이 시간을 buildTime이라고 한다. <br>

<br><br>

### final
> buildTime을 알고 있지 않아도 된다.
```
//아래 코드가 실행된 시간을 기준으로 저장된다.
final DateTime now = DateTime.now();
print(now);
```

<br><br>

### const
> buildTime을 알고 있어야 된다.
```
//compile error
const DateTime now = DateTime.now()
//언제 위 코드가 실행될지 모르기 때문이다.
```