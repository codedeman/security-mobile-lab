them code commit C1
them code commit C2
them code commit B2
them code commit B3
them code commit B4


```swift

    var world = "Hello world"
    var worldCoppy = world

    var arr1:Array = ["Kevin","Hieu"]
    var arr2 = arr1

    print(NSString(format: "%p", address(o: &world))) // ->0x10083c810

    print(NSString(format: "%p", address(o: &worldCoppy))) // ->0x10083c820



    print(NSString(format: "arr %p", address(o: &arr1))) // -> 0x109299fc0
    print(NSString(format: "arr %p", address(o: &arr2)))
 
```
