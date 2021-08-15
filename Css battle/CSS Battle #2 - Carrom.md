
# 1. Not so correct `Inline blocks`

*What is Inline Blocks?*
**`display: inline-block` allows to set a width and height on the element**

<table>
	<tr>
		<th>Picture</th>
		<th>Code</th>
 	</tr>
 	<tr>
  		<td>   
        <a href="https://imgbb.com/">
        <img width="140" height="100" src="https://i.ibb.co/MPf5VWz/Screenshot-5.png" alt="Screenshot-5" border="0" >
    </td>
   	<td> 

 ```html    
  span.b {
  display: inline-block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow; }  
  ```
    
  </td>
 	</tr>
</table>

``` html
<div id="a"></div>
<div id="b"></div>
<div id="c"></div>
<div id="d"></div>

<style>
  body{margin:0;  display: inline-block; padding:50px; background:#62374e}
  div{width:50px;height:50px;background: #fdc57b;}
  #b {margin-top: 100px;}
  #c {margin-left:250px;margin-top: -200px;}
  #d {margin-left:250px;margin-top: 100px}
</style>
```
# 2. Not correct `Inline blocks` ?

**Incorrect Part: The cubes dont match**

``` html
<div id="a"></div>
<div id="b"></div>
<div id="c"></div>
<div id="d"></div>

<style>
  body{margin:0;  display: inline-block; background:#62374e}
  div{width:50px;height:50px;background: #fdc57b;display:inline-block;}
  #a {margin-left:50px; margin-top: 50px;}
  #b {margin-left:200px; margin-top:50px;}
  #c {margin-left:50px;margin-top: 100px;}
  #d {margin-left:200px;margin-top: 100px}
</style>
```
# 3. Position: Fixed
*What is Position Fixed?*
`position`specifies the type of positioning method used for an element
-   `static`
-   `relative`
-   `fixed`
-   `absolute`
-   `sticky`
|Name|Idea| Picture |
|--|--|--|
| position:static; | Positioned according to page  |  |
| position: relative; | positioned relative to its normal position. |  |
| position: fixed;  |  |  |
| position: absolute;  |  |  |
| position: sticky;  |  |  |



```html
<div id="a"></div>
<div id="b"></div>
<div id="c"></div>
<div id="d"></div>

<style>
  body{margin:0;  display: inline-block; background:#62374e}
  div{width:50px;height:50px;background: #fdc57b;position:fixed;}
  #a {top:50; left:50;}
  #b {top:50; left:300;}
  #c {top:200; left:50;}
  #d {top:200; left:300;}
</style>
```

https://www.tablesgenerator.com/markdown_tables


> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbODgxNzU4MTU3LDEwNTk2NjQ2MTddfQ==
-->