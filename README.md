# Trillo
Second project of Advanced CSS Course. Link to course: https://www.udemy.com/course/advanced-css-and-sass

Below are a few notes to help understand some concepts and elements used in this project.

To install all required packages, run command **npm install** 

**Flexbox container**
```css
display: flex;

flex-direction: row; 
  /*
    - specifies direction of items
    row: normal flex order
    row-reverse: reverse direction of main axis
    column: order in columns
    column-reverse;: reversed order in columns
  */
  
  flex-wrap: wrap;
  /*
    - defines wrapping
    nowrap:
    wrap: will create new lines for items that dont fit container
    wrap-reverse;
  */
  
  justify-content: center;
  /*
    - defines alignment along main axis
    flex-start: puts items on the left side
    center: positions items into the middle of container
    space-between: evenly distributes space among items,
      divides all available space between elements
    space-around: puts the same amount of space on both sides od the items
    space-evenly: all spaces between items are always the same
    flex-end: puts items on the right side
  */
  
  align-items: center;
  /*
    - defines alignment along cross axis
    stretch: stretches all elements to match the highest item
    center: center elements on cross axis, based on biggest item
    flex-start: aligns items at the top of cross axis
    flex-end: aligns items at the end of cross axis
    baseline: aligns the text of the items, like invisible line under text
  */
  
  align-content: space-between;
  /* 
    - applies where there is more than 1 row
    stretch: initial value
    flex-start: aligns rows on top of cross axis 
    flex-end: aligns rows on bottom of cross axis
    center: center vertically
    space-around: distributes space between the rows, same space on top and bottom of the rows
    space-between: one of the lines on top, other on the bottom
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
  - flexbox orders elements based on order number; initial value is 0 
*/

flex-grow: 1; 
/* 
  0: item doesn't grow
  1: all items occupy entire space they possibly can
*/

flex-shrink: 0;
/*
  - defines how much an element is allowed to shrink
  0: element is not allowed to shrink
  1: initial value - element is allowed to shrink
*/

flex-basis: 300px;
/*
  - defines base width of item
*/

flex: 0 1 300px; /*shortcut for grow, shrink and basis */
```
