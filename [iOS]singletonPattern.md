# Singleton Pattern

특정 용도로 객체를 하나만 생성하여, 공용으로 사용하고 싶을 때 사용하는 디자인 유형

프로그램이 실행되고 끝날 때까지 특정용도를 가지는 단 하나의 객체를 만들어 놓고 쓰게되는 것임. (임의로 해제하지 않는 이상)

주로 환경설정, 로그인 정보, 유저 정보 등을 한 객체에 생성해 두고 여러 객체에서 공유해서 데이터를 쓸 수 있는 방법이다.

```
// 싱글턴 구현 방법
final class MySingleton {
  static let shared = MySingleton() // 정적 상수 생성
  
  var number = 0
  private init() {} // 새로운 인스턴스 생성을 막아버림!
}

let singleA = MySingleton.shared
let singleB = MySingleton.shared

print(singleA.number) // 0
print(singleB.number) // 0
singleA.number = 2
print(singleA.number) // 2
print(singleB.number) // 2
singleB.number = 7
print(singleA.number) // 7
print(singleB.number) // 7
// ** 모두 동일한 인스턴스를 가리키고 있다는 것을 확인할 수 있음!
```

```
struct MySingleton { // 구조체임!
  static let shared = MySingleton()
  
  var number = 0
  private init() {}
}

var singleA = MySingleton.shared
var singleB = MySingleton.shared

print(singleA.number) // 0
print(singleB.number) // 0
singleA.number = 2
print(singleA.number) // 2
print(singleB.number) // 0
singleB.number = 7
print(singleA.number) // 2
print(singleB.number) // 7
// ** 값 타입은 인스턴스가 공유되지 않음 (제각각)
```


-------
https://babbab2.tistory.com/66
https://medium.com/@Jager-yoo/swift-%EB%8B%A4%EC%8B%9C-%EA%B3%B5%EB%B6%80%ED%95%98%EB%8A%94-%EC%8B%B1%EA%B8%80%ED%84%B4-singleton-%ED%8C%A8%ED%84%B4-a013757775bc
