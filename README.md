# Simple Flex

Simple flex is a utility built to ease layout development with flex box
It has classes made to simplify layout development using classes only



## Basic usage

Just add `sf` class to the element and then add any of the alignment classes.
for example:
```html
<nav class="sf msb">
    <a class=""></a>
    <a class=""></a>
    ...
</nav>
```

Add the following classes for advanced use:
 - `column` - Convert the container a column
 - `inline` - Convert the container to a inline-flex element
 - `wrap` - make the elements in the container wrap when there is not enough space



## Alignment

Simple flex gives you a list of simple classes to align your content in the container
```
       t - top      |l - left
                    |
                    |
---------------------------------------
                    |
     m - middle     |    c - center
                    |
---------------------------------------
                    |
                    |
     b - bottom     |        r - right
```

Using combinations of those classes you can align the content of the container in any direction.
Simple flex also has built in combinations of all the alignment classes allowing you to easily
control positioning of the content in your container
```
                    |                      |
    tl - top left   |    tc - top center   |   tr - top right
                    |                      |
------------------------------------------------------------------
                    |                      |
  ml - middle left  |  mc - middle center  |  mr - middle right
                    |                      |
------------------------------------------------------------------
                    |                      |
  bl - bottom left  |  bc - bottom center  |  br - bottom right
                    |                      |
```

Simple flex also supports advanced flex based alignment:
```
.sb - space-between
.tsb - top space-between
.msb - middle space-between
.bsb - bottom space-between

.sa - space-around
.tsa - top space-around
.msa - middle space-around
.bsa - bottom space-around
```



## Columns

Simple flex has support for basic grids, it has an optional 12 columns grid, use classes c1-c12 for column width:
```html
<div class="sf">
    <div class="c6">column 1/2</div>
    <div class="c6">column 1/2</div>
</div>
<div class="sf">
    <div class="c4">column 1/3</div>
    <div class="c4">column 1/3</div>
    <div class="c4">column 1/3</div>
</div>
<div class="sf">
    <div class="c4">column 1/3</div>
    <div class="c8">column 2/3</div>
</div>
<div class="sf">
    <div class="c3">column 1/4</div>
    <div class="c3">column 1/4</div>
    <div class="c3">column 1/4</div>
    <div class="c3">column 1/4</div>
</div>
```
```
|                             |                             |
|         column 1/2          |         column 1/2          |
|                             |                             |
-------------------------------------------------------------
|                   |                   |                   |
|    column 1/3     |    column 1/3     |    column 1/3     |
|                   |                   |                   |
-------------------------------------------------------------
|                   |                                       |
|    column 1/3     |               column 2/3              |
|                   |                                       |
-------------------------------------------------------------
|              |              |              |              |
|  column 1/4  |  column 1/4  |  column 1/4  |  column 1/4  |
|              |              |              |              |
```



## Spacing

Use the `spacing` class to add spacing between the element in the container.
works for flex row or column
```html
<div class="sf spacing msb">
    <div>left</div>
    <div>right</div>
</div>
<div class="sf column spacing mc">
    <div>left</div>
    <div>center</div>
    <div>right</div>
</div>
```



## Installation
Simply import the css file to your project and start using Simple flex
```html
<link rel="stylesheet" href="//rawgit.com/dcohenb/simple-flex/master/simple-flex.css">
```
