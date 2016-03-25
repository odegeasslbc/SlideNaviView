# SlideNaviView
## A slide navi controller 

Integrated by UIView rather than UIViewController.

![alt tag](https://cloud.githubusercontent.com/assets/9973368/13720709/9fddf2ce-e7dd-11e5-97cf-839f76330af5.gif)

![alt tag](https://cloud.githubusercontent.com/assets/9973368/13720710/a0fd8ff2-e7dd-11e5-8a84-aef7da05fa91.gif)

##USAGE
###Initialize
```swift
let slideNaviView = SlideNaviView(frame: CGRect) 
```

###Modification
```swift
slideNaviView.modifyMainViewUnit(atIndex: 2, operation: {view in view.backgroundColor = UIColor.blueColor()})
slideNaviView.modifyLabelUnit(atIndex: 0, operation: {label in label.text = "一"})
```
        
###Add unit views
```swift

//initialize reach sub views

var firstView = UIView(frame: CGRectMake(0, 2, 20, 20))

firstView.backgroundColor = UIColor.greenColor()

var secondView = UIView(frame: CGRectMake(0, 2, 20, 20))

secondView.backgroundColor = UIColor.greenColor()

var thirdView = UIView(frame: CGRectMake(0, 2, 20, 20))

third.backgroundColor = UIColor.greenColor()

var tmp = [UIView]()

tmp.append(firstView)

tmp.append(secondView)

// sub views can be inserted directly
slideNaviView.insertMainView(2, view: thirdView)
// sub views can also be inserted together as an array of views
slideNaviView.setMainViews(tmp)
```
