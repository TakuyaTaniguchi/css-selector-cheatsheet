# css-selector-cheatsheet


https://coliss.com/articles/build-websites/operation/css/css-selectors-cheatsheet.html

## Tag

### Dependence 1 0 0
**main**

``` SCSS
div {
    foo: bar;
}

p{
  foo: bar;
}


body div{
  foo: bar;
}

```



``` SCSS
.button{
    foo: bar;//base
    &.-mod-active{
        color: red;//active
    }
     &:not(.-mod-active){
        color: gray;//inactive
    }
    
}

```
