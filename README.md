# CirculoMenu
Simple menu with a circular layout.

# Usage
1. Create `UIView` in your storyboard or programatically.
2. Specify `CircleMenuView` for your `UIView`.
3. Configure menu: specify menu button, items and handler.
```
circleMenuView.centerButton = CircleMenuButton(
 id: "main",
 image: "plus",
 color: Color(val: 0x7C93FE)
)

// circle buttons
circleMenuView.buttons = [
 CircleMenuButton(
  id: "exchange_id",
  image: "exchange",
  color: Color(val: 0x9F85FF)
 ),
 ...
 CircleMenuButton(
  id: "visa_id",
  image: "visa",
  color: Color(val: 0xF55B58)
 )
]
  
// distance between center button and buttons
circleMenuView.distance = 90.0

// animation duration
circleMenuView.duration = 0.35

// show buttons on the half circle
circleMenuView.halfMode = true
```

## Installation

### [CocoaPods](http://cocoapods.org)

To install it, simply add the following line to your Podfile:
```ruby
pod "CirculoMenu", "0.6.0"
```

### [Carthage](http://github.com/Carthage/Carthage)

```ogdl
github "Exyte/CirculoMenu" ~> 0.6.0
```

### Manually

Drop [CircleMenuView.swift](https://github.com/exyte/CirculoMenu/blob/master/Circulo/CircleMenuView.swift) in your project.

## Requirements

* iOS 8.0+ / Mac OS X 10.9+
* Xcode 7.3+
