Swift Snippets
=============

A collection of Swift snippets I've found useful when starting out with the language. These are things that tripped me up due to not reading the Swift Programming Language book enough.

### Getting used to closures with UIView Animations

```swift
UIView.animateWithDuration(1.0, animations: {() -> Void in
  // Animations
})
```

Which can be simplified to 

```swift
UIView.animateWithDuration(1.0, animations: {
  // Animations
})
```

Which after reading the docs more, if a closure is the last argument then you can just pass it after the call

```swift
UIView.animateWithDuration(1.0) {
  // Animations
}
```

Closures with return types are called like so

```swift
UIView.animateWithDuration(1.0, animations: {
  // Animations
}, completion: { success in
  // Completion
})
```
