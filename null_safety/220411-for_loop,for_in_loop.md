## for_loop
- for(초기값; 조건값; 증가값){ }
```
for(int i = 0; i < 10; i++){
    print(i);
    //1
    //2
    //3
    //4
    //5
    //6
    //7
    //8
    //9
}
```
<br><br>

> List num의 모든 요소값 더하기 <br>
```
void main(){
    int tot = 0;
    List<int> num = [1, 2, 3, 4, 5, 6];
    
    for(int i = 0; i < num.length; i++){
        tot += num[i];
    }
    print(tot); //21
}
```
<br><br><br>

## for_in_loop
- for(넣어질 변수 in 넣을 변수){ }
```
void main(){
    List<int> num = [1, 2, 3, 4, 5, 6];
    for(int nums in num){
        print(nums);
        //1
        //2
        //3
        //4
        //5
        //6
    }
}
```