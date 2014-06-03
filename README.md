Swift Snippets
=============

A collection of Swift snippets I've found useful when starting out with the language. These are things that tripped me up due to not reading the Swift Programming Language book enough.

### UIView Animations

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

Closures with return types are called like so

```swift
UIView.animateWithDuration(1.0, animations: {
  // Animations
}, completion: { success in
  // Completion
})
```
