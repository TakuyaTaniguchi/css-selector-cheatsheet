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

### :not selector usecase
https://codepen.io/Rin_T_T/pen/ZEERzbe  
**main**

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

https://codepen.io/Rin_T_T/pen/ZEERzbe  
**main**

``` SCSS
.not{
  ul{
    li{
      & + li {
        margin-top: 15px;
      } 
    }
  }
}

.good{
  ul{
    li{
      &:not(:first-of-type){
        margin-top: 15px;
      } 
    }
  }
}

```
