# Trillo
Second project of Advanced CSS Course

To install all required packages, run command **npm install** 

**Flexbox container**
```css
display: flex;

flex-direction: row; 
  /*
    row: initial value, normal flex order
    row-reverse: reverse direction of main axis
    column: order in columns
    column-reverse;: reversed order in columns
  */
  
  justify-content: center;
  /*
    center: positions items into the middle of container
    space-between: evenly distributes space among items
    space-around: puts the same amount of space on both sides od the items
    space-evenly: all spaces between items are always the same
    flex-end: puts items on the right side
    flex-start: default values - puts items on the left side
  */
  
  align-items: center;
  /*
    center: center elements on cross axis, based on biggest item
    flex-start: aligns items at the top of cross axis
    flex-end: aligns items at the end of cross axis
    stretch: stretches all elements to match the highest item
    baseline: aligns the text of the items, like invisible line under text
  */
  
  flex-wrap: wrap; /* will create new lines for items that dont fit container */
  /*
    nowrap, wrap, wrap-reverse
  */
  
  align-content: space-between;
  /* 
    flex-start: aligns rows on top of cross axis 
    flex-end: aligns rows on bottom of cross axis
    center: center vertically
    space-around: distributes space between the rows, same space on         top and bottom of the rows
    space-between: one of the lines on top, other on the bottom
    stretch: initial value
  */
```

**Flexbox item**
```css
align-self: flex-end;
/*
  - aligns this specific item
  auto
  stretch
  flex-start
  flex-end
  center
  baseline
*/

order: 1; 
/*
  flexbox orders elements based on order number; initial value is 0 
*/

flex-grow: 1; 
/* 
  0: initial value, item doesn't grow
  1: all items occupy entire space they possibly can
*/

flex-shrink: 0;
/*
  defines how much an element is allowed to shrink
  0: element is not allowed to shrink
  1: initial value - element is allowed to shrink
*/

flex-basis: 300px;
/*
  defines base width of item
*/

flex: 0 1 300px; /*shortcut for grow, shrink and basis */
```
