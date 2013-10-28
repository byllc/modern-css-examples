Modern CSS Examples
===================

 Example CSS 3 tricks that are starting have adequate browser support. These should all work on the latest version of the major browsers. Most have worked for several generations of chrome or webkit based browser in general. 

Gradient
--------
```css
  
  background: linear_gradient(to bottom, red, blue)
  background: radial_gradeint(red,blue)
```

Columns
-------
```css
  -moz-columns:3;
  -webkit-columns:3;
  columns:3;  
```

Value Calculation
-----------------
```css
  /* Can use with any length or size attribute */
  width: calc(100% - 40px);
```

Before And After
----------------
```css
selector::before{
  content:'Defined via CSS-- ';
}

selector::after{
  content:' --Defined via CSS';
}
```
Animations
----------
```css
.animator_container{
  position: relative;
  height: 200px;
}

.animator{
  width:100px;
  height:100px;
  background:purple;
  position: absolute;
  animation:myAnimation 20s;
  -webkit-animation:myAnimation 20s; /* Safari and Chrome */
}

@keyframes myAnimation{
  0%   {background: purple; left: 0px; top:10px;}
  25%  {background: yellow; left:400px; top:10px;}
  50%  {background: blue; left:400px; top:100px;}
  75%  {background: green; left:0px; top:100px;}
  100% {background: black; left:0px; top:10px;}
}

@-webkit-keyframes myAnimation{ /* Safari and Chrome */
  0%   {background: purple; left: 0px; top:10px;}
  25%  {background: yellow; left:400px; top:10px;}
  50%  {background: blue; left:400px; top:100px;}
  75%  {background: green; left:0px; top:100px;}
  100% {background: black; left:0px; top:10px;}
}
```

Rounded Corners
---------------
```css

 -moz-border-radius: 30px;
 -webkit-border-radius: 30px;
 -khtml-border-radius: 30px;
 border-radius: 30px;
```

Counters
--------
```css

body {
  counter-reset: section;  /* Set to 0 */
}

p:before {
  counter-increment: section;  
  content: "Section " counter(section) ": " 
}
```

