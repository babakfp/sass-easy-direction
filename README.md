# easy-dir
A CSS library for easily create separate RTL and LTR css style files.


## Sync

###### direction

``` direction: e(rtl) ``` => ``` direction: ltr ```

``` direction: e(ltr) ``` => ``` direction: rtl ```


###### left and right
``` prop-#{e(left)}: ```    => ``` prop-right: ```

``` prop-#{e(right)}: ```   => ``` prop-left: ```

``` prop: e(left) ```       => ``` prop: right ```

``` prop: e(right) ```      => ``` prop: left ```


###### positive and negative

``` prop: e(-10px) ``` => ``` prop: 10px  ```

``` prop: e(3rem) ```  => ``` prop: -3rem ```


###### translate

``` transform: translate(30px, 10px) ``` => ``` transform: translate(-30px, 10px) ```

``` transform: translate(-20%, 10%) ```  => ``` transform: translate(20%, 10%) ```


###### translateX

``` transform: translateX(30px) ``` =>  ``` transform: translateX(-30px) ```

``` transform: translateX(-20%) ``` => ``` transform: translateX(20%) ```



## Variables


###### turn on/off functionality.

``` $eActive: true !default; ```


###### direction than you want to styles be convert.

``` $eConvertTo: rtl !default; ```


###### this will disable css prop value translate.

``` $eTranslate: true !default; ```


###### this will disable css prop value translateX.

``` $eTranslateX: true !default; ```



## How to use
Use the sass functions that I created, in your project. in the end, export a .css file named RTL(for original ltr projects) or ltr(for original RTL projects). load specific direction to specific countries.
All .scss files are required to include it in your project.



## New update detiles
- Add new function named 'e()' to control output.
- Add new 'e4()' function to control props with 4 values like:margin,padding.
- Remove lr, pn, dir functions.
- Change variables name located in variables folder.