# easy-direction
A CSS library to easily convert styles from LTR```to```RTL and RTL```to```LTR.


## How it works?
This library will give you a sass/scss function named e(). give your value as a prop to this functin and it will carry all heavy stuff.

```scss

.direction {
  direction: e(ltr);
  direction: rtl; // output
}

.left-and-right {
  float: e(left);
  float: right; // output

  margin-#{e(left)}: 1rem;
  margin-right: 1rem; // output
}

.positive-and-negative-values {
  right: e(-1%);
  right: 1%; // output
}

.translate-and-translateX {
  transform: translate(1px, 1px);
  transform: translate(-1px, 1px); // output

  transform: translateX(1rem);
  transform: translateX(-1rem); // output
}
// ^ for this you dont need to use e() function.

```


## Variables
```scss

// turn on/off conversion
$is-active: true !default;

// smart translate. this will disable pure css translate|translateX functionality.
$activate-translate: true !default;
$activate-translate-x: true !default;

```

## How to use
Download and import ```src/index``` file in your project ;)
There is a demo file to help you understand how all works.