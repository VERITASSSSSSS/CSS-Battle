# 1. Easy and Stupid
```css
<div class="c"></div>
<div class="b"></div>
<div class="a"></div>
<style>
  *{background: #0B2429;}
  div {
    position: absolute;
    top: 150px;left:85px;
    width: 115px;height: 120px;
    background: #F3AC3C;
    border-radius:160% 0 180% 155%;
  }
  .b{top:90px; left:145; background:#998235;}
  .c{width: 120px;height: 120px;top:30px; left:200; border-radius: 50%;}
  
</style>
```

# 2. Z-index
*What is z-index ?*
**`z-index: 1;` specifies the stack order of an element.

```css
<div id="o">
  <div id="a"></div>
  <div id="b"></div>
  <div id="c"></div>
</div>
<style>
  *{margin:0; background:#0B2429;}
  
  #o{margin: 30px 80px; 
	 width: 250px; height: 240px;}
	 
  #o div{width: 120px; height:120px; 
		 position: absolute;}
  
  #a{margin: 0px 120px;
    z-index:1; 
    background: #F3AC3C;
    border-radius: 60px;}
  
  #b{z-index: 2;
     margin: 60;
     background: #998235;
     border-radius: 60px 0px 60px 60px;}
  
  #c{z-index: 3;
     margin: 120 1;
     background: #F3AC3C;
     border-radius: 60px 0px 60px 60px;}
 </style>
```

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2ODM3OTc4NTgsLTE3OTQ4OTA2NjRdfQ
==
-->