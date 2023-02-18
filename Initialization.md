# Initialization (초기화)



초기화를 알기 위해서는 일단 상속이란 개념을 알아야한다.

초기화는 클래스, 구조체



## init을 하는 이유
어찌보면 당연한거라고 할 수 있는데, 새로운 인스턴스를 생성하기 위해서다. 블루프린트 같은 struct를 복사해서 사용하려면
결국 init을 해서 초기값을 할당해야하는 거다. 만약 초깃값을 안주면 구조체의 인스턴스를 생성할 때마다 값을 줘야하니까 말이 안됨
```swift
struct Person {
    var firstName: String
    var middleName: String
    var lastName: String
    let ethnicity: String
    var height: Int
    var weight: Int
}
let me = Person(firstName: <#T##String#>, middleName: <#T##String#>, lastName: <#T##String#>, ethnicity: <#T##String#>, height: <#T##Int#>, weight: <#T##Int#>)
```
손나칸지..

이해한 시점에서 생각해보니 새로운 개념이라 처음에 못 알아들은 것 같다.. 역시 써봐야한다.
