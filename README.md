Simple  fluid Sass grid
================

This is a very simple Sass grid system module. 

It requires setting 2 variables:

$siteMaxWidth - maximum width of the site

$columnMaxGutter - size of a gutter between 2 columns, when site is in maximum width

##Usage

Module allows using 2 placeholders and 1 mixin.

%siteWrapper - to be extended by site wrapper

example:
```html
  #wrapper{ @extend %siteWrapper}
```

%gridRow - to be extended by all grid rows - column wrappers

example:
```html
  .main{ @extend %gridRow}
```

@mixin gridCol($fraction) - main mixin for creating grid columns - it takes a $fraction as an argument to calculate the required width.

example:
```html
  .sidebar{ @include gridCol(1/4)}
```

###Demo
http://www.logconsole.com/samples/simple-fluid-sass-grid/