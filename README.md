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
