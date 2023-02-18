# Combine

api call할 때 사용한다고 생각하면 편합니다. "도대체 Swift는 어떻게 api call 비동기 처리하는거야!" 할 때 공부해야 할 것이 Combine입니다.

## Publisher
프로토콜입니다. 하나 이상의 Subscriber인스턴스에게 element를 제공합니다.

## Subscriber
역시나 프로토콜입니다. Publisher로부터 input을 받을 수 있는 타입을 선언하는 프로토콜입니다.
Subscriber 인스턴스는 Publisher의 element stream, 그들의 relationship의 변경사항을 설명하는 lifecycle이벤트를 받습니다.


## Subject

## Scheduler

## Cancellable
