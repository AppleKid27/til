
* Publisher 送信する側
* Subscriber 受け取る側
* Operator 受信時に処理を加工する

```Swift
// Publisher
let subject = PassthroughSubject<Int, Never>()

subject
    // Operator
    .map { String($0) }
    // Subscriber
    .sink { value in
        print(value)
    }

// Publisherのイベントの送信
subject.send(0)
subject.send(1)
subject.send(2)
```
