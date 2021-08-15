# 1. Absolute Position

*What is `:before`?*
The `::before` and `::after` pseudo-elements in CSS allows you to insert content onto a page without it needing to be in the HTML.
```css
<div id="a"></div>
<div id="b"></div>
<div id="c"></div>

<style>
  *{
    background: #62306D;}
  
  div{
   width: 100px;height:100px;
   background: #F7EC7D;
   position: absolute;
   border-radius: 0 0 50px 50px;
  }
  #a{top:150px;left:50px;}
  #b{transform:rotate(180deg);top:50px;left:150px;}
  #c{top:150px;left:250px;}
  
</style>
```

# 2. Border

## Concept

*What is `transform: translate`?*
- Use it to center
-   move me leftwards by 50% of my width, along the x-axis, and
-   move me upwards by 50% of my height, along the y-axis
- 
[Transform: translate](https://stackoverflow.com/questions/46184458/transform-translate-50-50/46184660)

### Code
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

### Break it down

```css
  #rect{
   width: 300px;height:150px;
   margin:75px 50px; 
   background: #243D83;
   overflow: hidden;
   position: relative;
  }
```

- Adding `position: relative` to `rect` as the immediate parent of `outer` makes the circle follow the center of the rectangle.

- `overflow: hidden` which in this case doesn't seem to have an effect because the border of the outer circle has the same color as the background.

```css
  #inner{
    width: 50px;height:50px;
    border-radius: 25px;
    margin: 50px auto;
    background:#EEB850;
  }
  ```
  
- If the  `margin`  property has two values:
	-   **margin: 25px 50px;**
	    -   top and bottom margins are 25px
	    -   right and left margins are 50px
	    
- set the margin property to `auto` to **horizontally** center the element within its container.

[Centering in CSS](https://css-tricks.com/centering-css-complete-guide/)

# 3. Box Shadow

**Style**
```css
box-shadow: [horizontal offset] [vertical offset] 
[blur radius] [optional spread radius] [color];
```
```css
<div id="rect">
  <div id="circle">
  </div>
</div>

<style>
  body{
    background: #6592CF}
  
  #rect{
   width: 300px;height:150px;
   margin:75px 41px; 
   background: #243D83;
   display: flex; 
   justify-content: center;
    align-items: center;
  }
  
  #circle{
    width: 50px;height:50px;
    border-radius: 25px;
    margin: 50px auto;
    box-shadow: 0 0 0 50px #243D83,0 0 0 100px #6592CF;
    background:#EEB850;
  }
  
</style>
```

> Written with [StackEdit](https://stackedit.io/).

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDEwNTYwNjIsLTk0NjAzNDcxNCwtMjg5Nj
QwMzQ5LC0xMTIxNzA4MTMsMTM2NTQ1NDQzOSwxMzA1MjMzNTgz
LC0xMDY1MDI2NjE0LC0xMjMxMzg2MTE5XX0=
-->