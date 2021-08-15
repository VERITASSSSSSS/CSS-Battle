# 1. Slow and Stupid

*What is `:before`?*
The `::before` and `::after` pseudo-elements in CSS allows you to insert content onto a page without it needing to be in the HTML.
```css
div::before { content:  "before";  }  
div::after  {  content:  "after";  }
```
```html
<div> 
before 
<!-- Rest of stuff inside the div --> 
after 
</div>
```
[:after / :before](https://css-tricks.com/almanac/selectors/a/after-and-before/)
```html
<div id="c"></div> <!--Right piece-->
<div id="d"></div> <!--Left piece-->
<div id="b"></div> <!--Small circle-->
<div id="a"></div> <!--Big circle-->

<style>
  body{margin:0;  
    display: inline-block; 
    background:#6592CF}
  
  div{width:50px;
    height:50px;
    background: #243D83;
    position:absolute;}
  
  
  #a {border-radius:50%; 
    left:175px; top:125px;
    background:#EEB850; }
  
  #b {border-radius:50%; 
    width:150px;height:150px; 
    left:125px; top:75px;
    background:#243D83; }
  
  #c {width:50px;height:150px; 
    left:50px; top:75px;}
  #d {width:50px;height:150px; 
    left:300px; top:75px;}
  
    #d:before{
    content:" ";
    position: absolute;
    width: 250px; height: 250px;
    left: -225px;top: -50px;
  	border-radius: 50%;
	background:#6592CF;
  }
</style>
```

# 2. Border

## Concept


*What is `:before`?*
The `::before` and `::after` pseudo-elements in CSS allows you to insert content onto a page without it needing to be in the HTML.
```css
div::before { content:  "before";  }  
div::after  {  content:  "after";  }
```
```html
<div> 
before 
<!-- Rest of stuff inside the div --> 
after 
</div>
```
[:after / :before](https://css-tricks.com/almanac/selectors/a/after-and-before/)
```html
<div id="rect">
  <div id="outer">
    <div id="inner"></div>
  </div>
</div>

<style>
  body{
    margin:0;
    background: #6592CF}
  
  #rect{
   width: 300px;height:150px;
   margin:75px 50px; 
   background: #243D83;
   overflow: hidden;
   position: relative;
  }
  
  #outer{
    border: 50px solid #6592CF;
    border-radius: 150px;
    width: 150px;height:150px;
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%,-50%);
    background:#243D83;
  }
  
  #inner{
    width: 50px;height:50px;
    border-radius: 25px;
    margin: 50px auto;
    background:#EEB850;
  }
  
</style>
```

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQyNjgwMDQ3NywtMTA2NTAyNjYxNCwtMT
IzMTM4NjExOV19
-->