Angular 1 Pin Code Directive
==============

A simple Angular 1 directive to draw a n digit pin input.

![alt tag](https://github.com/VitorMFMarques/angularpincode/blob/master/image.png)

How to use?
==============

Add module <b>pinCode</b> to your app module dependencies.

Add an element of type pin.
```html
<pin digits="4" pin="pin"></pin>
```

Options
==============
Name    | Description | Mandatory | Default Value
 -------| ----------- | --------- | --------
pin | scope varible where the pin value will be binded | Yes | NA
digits | number of digits | No | 4
hide-input | hide input value after inserted | No | true
hide-timeout | time after which the input value will be hidden | No | 200 (ms)
hide-symbol | symbol used to show when the input is hidden (HTML Symbol Entities) | No | &#9899; (&#9899)
on-enter | function called when user press enter after the last digit insertion | No | NA

Events
==============

To focus in an input, broadcast the event 'focusPin' with the object {digitIndex:x}
```html
$scope.$broadcast('focusPin',{digitIndex:0});
```
