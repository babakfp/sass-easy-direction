# easy-dir
A CSS library for easily create separate RTL and LTR css style files.


## Sync

###### direction

``` direction: dir(rtl) ``` => ``` direction: ltr ```

``` direction: dir(ltr) ``` => ``` direction: rtl ```


###### left and right
``` prop-#{ lr(left) }: ```  => ``` prop-right: ```

``` prop-#{ lr(right) }: ``` => ``` prop-left: ```

``` prop: lr(left) ```       => ``` prop: right ```

``` prop: lr(right) ```      => ``` prop: left ```


###### positive and negative

``` prop: pn(-10px) ``` => ``` prop: 10px  ```

``` prop: pn(3rem) ```  => ``` prop: -3rem ```


###### translate

Sass function that are used for this prop, are same name with original css prop value name. 

``` transform: translate(30px, 10px) ``` => ``` transform: translate(-30px, 10px) ```

``` transform: translate(-20%, 10%) ```  => ``` transform: translate(20%, 10%) ```


###### translateX

Sass function that are used for this prop, are same name with original css prop value name. 

``` transform: translateX(30px) ``` =>  ``` transform: translateX(-30px) ```

``` transform: translateX(-20%) ``` => ``` transform: translateX(20%) ```



## Variables


###### turn on/off functionality.

``` $easyDir: true !default; ```


###### direction than you want to styles be convert.

``` $easyDir-dir: rtl !default; ```


###### this will disable css prop value translate.

``` $easyDir-translate: true !default; ```


###### this will disable css prop value translateX.

``` $easyDir-translateX: true !default; ```



## How to use
Use the sass functions that I created, in your project. in the end, export a .css file named RTL(for original ltr projects) or ltr(for original RTL projects). load specific direction to specific countries.
All .scss files are required to include it in your project.