# View Controller

application은 Window, View Controller, View로 이루어져있다.

<img width="667" alt="image" src="https://user-images.githubusercontent.com/53306921/219932080-07a26a73-6f20-4c46-bfce-f1e80b8452dd.png">


## Window (UIWindowScene)
Window는 최상위 container다. 여기서 window를 하나라고만 생각할 수 있는데, 모든 애플리케이션은 
최소 하나 이상의 window와 view가 존재한다.
```
A scene that manages one or more windows for ur app
```

## View (UIView)
View는 중첩될 수 있고, 계층 구조를 이루는데  parent view(superview), child view(subview)로 이루어져있다.
걍 뷰는 말그대로 뷰..
```
An object that manages the content for a rectangular area on the screen
```

## View Controller ([UIViewController](https://developer.apple.com/documentation/uikit/uiviewcontroller))
View Controller는 뷰를 관리한다.
말그대로 뷰를 컨트롤 하는거다.
```
An object that manages a view hierarchy for ur UIKit app
```
