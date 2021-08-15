# 1. Slow and Stupid

*What is Inline Blocks?*
**`display: inline-block` allows to set a width and height on the element**

<div id="c"></div> <!--Right piece-->
<div id="d"></div> <!--Left piece-->
<div id="b"></div> <!--Small circle-->
<div id="a"></div> <!--Big circle-->

```html
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

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQzMzcxMzY1Nl19
-->