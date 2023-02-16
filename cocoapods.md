# cocoapods

react로 치면 라이브러리 쓸 수 있는 방법이 몇 가지 있는데 그 중 하나가 cocoapods이다.
https://cocoapods.org/
여기 들어가면 npm처럼 많이 모여있음.

프로젝트에 라이브러리 사용하고 싶으면

```
$ sudo gem install cocoapods
```
하고 프로젝트에 들어가서 

```
vi Podfile
```
해서 팟파일 열고 
```
pod install
```
해주면 된다.


할려고 했는데 M1이라 또 arch 에러 떠서
https://stackoverflow.com/questions/71815618/swift-cocoa-pods-issue-library-ruby-gems-2-6-0-gems-ffi-1-15-5-lib-ffi-c-bund
이거로 해결해줌
