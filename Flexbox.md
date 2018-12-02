# FLEXBOX Cheatsheet/Guide

To use flex you need to declare ```display: flex``` in your css.

The following are the supporting properties for flexbox

## justify-content

Aligns items HORIZONTALLY and accepts the following values:

* flex-start: Items align to the left side of the container
* flex-end: Items align to the right side of the container
* center: Items align at the center of the container
* space-between: Items display with equal spacing BETWEEN them
* space-around: Items display with equal spacing ARROUND them

## align-items

Aligns items VERTICALLY and accepts the following values:

* flex-start: Items align to the top of the container
* flex-end: Items align to the bottom of the container
* center: Items align at the vertical center of the container
* baseline: Items display at the baseline of the container
* stretch: Items are stretched to fit the container

## align-self (for individual items)

Same as align-items but for an individual item to align itself.

## flex-direction

Defines the direction items are placed in the container, and accepts the following values:

* row: Items are placed the same as the text direction.
* row-reverse: Items are placed opposite to the text direction.
* column: Items are placed top to bottom.
* column-reverse: Items are placed bottom to top.


## order

Sometimes reversing the row or column order of a container is not enough. In these cases, we can apply the ``order: <integer>`` property to individual items. **By default, items have a value of 0,** but we can use this property to set it to a **positive or negative integer value**.

Lets say you have 3 items, by default they'll all have order 0. If you want to move one of those items to the leftmost you would need to set the order of that item to -1 or lower for it to be moved all the way to the left given that the order is lower than 0, same goes if you wish to move an item to the right; you would set the order to be 1 or higher. 

## flex-wrap

Spreads items depending on the following properties:

* nowrap: Every item is fit to a single line.
* wrap: Items wrap around to additional lines.
* wrap-reverse: Items wrap around to additional lines in reverse.

## flex-flow

The combination of ```flex-direction``` and ```flex-wrap``` since these two are used together so much. This property accepts the value of one of the two properties separated by a space.

E.G. ```flex-flow: row wrap``` or ```flex-flow: column nowrap```

## align-content

Set how multiple lines are spaced apart from each other. This property takes the following values:

* flex-start: Lines are packed at the top of the container.
* flex-end: Lines are packed at the bottom of the container.
* center: Lines are packed at the vertical center of the container.
* space-between: Lines display with equal spacing between them.
* space-around: Lines display with equal spacing around them.
* stretch: Lines are stretched to fit the container.
