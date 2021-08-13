# SASS Easy Direction
A SASS library that helps you to easily convert styles from LTR to RTL and RTL to LTR. You can create multi-language websites easily with this library, without worrying about the CSS that you write.

## How it works?
You are going to have 3 functions. `_()`, `translate()`, `translateX()` and 2 mixins `html-ltr`, `html-rtl`. Visit the demo file to learn how to use them.

### Variables
There is only 1 variable to worry about.
```sass
// turn on / off the functionalities of this library.
$is-dir-active: false !default
```

### How to use
```sass
@import "./path/sass-easy-direction" as *
```
