## Section 2 Reflections

### _7. Headings and Basic Typography_

Display headings as different headings: `<h4 class="h2"></h4>`  
Add subtext inside a header: `<small class="text-muted">Subtext<small>`  
Display (huge) headings: `<h1 class="display-1"></h1>`  
Lead paragraphs: `<p class="lead"></p>`  

Bold text: `<p class="font-weight-bold"></p>`  
Normal text: `<p class="font-weight-normal"></p>`  
Italic text: `<p class="font-italic"></p>`  

Text transforms:
```html
<p class="text-lowercase"></p>
<p class="text-uppercase"></p>
<p class="text-capitalize"></p>
```

A right-aligned blockquote with a footer:
```html
<blockquote class="blockquote text-right">
  <p>_Quote quote quote_</p>
  <footer class="blockquote-footer"> Someone famous in <cite
  title="Source Title"> Source Title </cite></footer>
</blockquote>
```

Unstyle a list:
```html
<ul class="list unstyled">
  <li> To remove </li>
  <li> bullets </li>
  <li> and padding. </li>
</ul>
```

Inline lists:
```html
<ul class="list-inline">
  <li class="list-inline-item"> Lorem ipsum </li>
  <li class="list-inline-item"> Lorem ipsum </li>
  <li class="list-inline-item"> Lorem ipsum </li>
</ul>
```


### _8. Text Alignment and Display_

Self-explanatory basic alignments:
```html
<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolor ad deleniti, placeat cumque, maiores fugiat tenetur ea voluptas voluptatem odio odit, dicta.</p>
<p class="text-left">Text aligned left</p>
<p class="text-center">Text aligned center</p>
<p class="text-right">Text aligned right</p>
```


Responsive alignments:
```html
<p class="text-sm-right">Right aligned on small or larger</p>
<p class="text-md-right">Right aligned on medium or larger</p>
<p class="text-lg-right">Right aligned on large or larger</p>
<p class="text-xl-right">Right aligned on xl or larger</p>

<p class="text-sm-left">Left aligned text on small or larger</p>
<p class="text-md-left">Left aligned text on medium or larger</p>
<p class="text-lg-left">Left aligned text on large or wider</p>
<p class="text-xl-left">Left aligned text on extra large or wider</p>

<p class="text-sm-center">Center aligned text on small or larger</p>
<p class="text-md-center">Center aligned text on medium or larger</p>
<p class="text-lg-center">Center aligned text on large or wider</p>
<p class="text-xl-center">Center aligned text on extra large or wider</p>
```


Vertical alignment:  
```html
<span class="align-baseline">baseline</span>
<span class="align-top">top</span>
<span class="align-bottom">bottom</span>
<span class="align-middle">middle</span>
<span class="align-text-top">text-top</span>
<span class="align-text-bottom">text-bottom</span>
```


Turn block into inline:  
```html
<h1 class="d-inline">Hello</h1>
<h1 class="d-inline">Goodbye</h1>
```


Turn inline into block:  
```html
<span class="d-block">Block</span>
```


Turn block into inline block:  
```html
<div class="d-inline-block">
  <h3>Hello</h3>
  This is inline
</div>
<div class="d-inline-block">
  <h3>Hello</h3>
  This is inline
</div>
```


### _9. Floats and Positions_

Basic floats:  
```html
<div class="float-left">Float left</div><br>
<div class="float-right">Float right</div><br>
<div class="float-none">Float none</div><br>
```


Responsive floats:  
```html
<div class="float-sm-right">Float right on small or wider</div><br>
<div class="float-md-right">Float right on medium or wider</div><br>
<div class="float-lg-right">Float right on large or wider</div><br>
<div class="float-xl-right">Float right on extra large or wider</div><br>

<div class="float-sm-left">Float left on small or wider</div><br>
<div class="float-md-left">Float left on medium or wider</div><br>
<div class="float-lg-left">Float left on large or wider</div><br>
<div class="float-xl-left">Float left on extra large or wider</div><br>

<div class="float-sm-none">Float none on small or wider</div><br>
<div class="float-md-none">Float none on medium or wider</div><br>
<div class="float-lg-none">Float none on large or wider</div><br>
<div class="float-xl-none">Float none on extra large or wider</div><br>
```


Clearfix:  
```html
<div class="clearfix">
    <button class="float-left">Float Left</button>
    <button class="float-right">Float Right</button>
</div>
```


Fixed and stickies:  
```html
<h3 class="fixed-top">Fixed Top</h3>
<h3 class="sticky-top">Sticky</h3>
<h3 class="fixed-bottom">Fixed Bottom</h3>
```
_Note: Fixed-top text is fixed to the top of the page at all times. Sticky-top sticks to the top once it hits the top of the page, and unsticks if you scroll up past its original position._

### _10. Colors and Background_

Text colors:
```html
<p class="text-primary">Text Primary Color</p>
<p class="text-secondary">Text Secondary Color</p>
<p class="text success">Text Success Color</p>
<p class="text-info">Text Info Color</p>
<p class="text-warning">Text Warning Color</p>
<p class="text-danger">Text Danger Color</p>
<p class="text-light">Text Light Color</p>
<p class="text-dark">Text Dark Color</p>
<p class="text-white">Text White Color</p>
```

Background colors:
```html
<div class="bg-primary">Background Primary Color</div>
<div class="bg-secondary">Background Secondary Color</div>
<div class="bg-success">Background Success Color</div>
<div class="bg-info">Background Info Color</div>
<div class="bg-warning">Background Warning Color</div>
<div class="bg-danger">Background Danger Color</div>
<div class="bg-light">Background Light Color</div>
<div class="bg-dark">Background Dark Color</div>
<div class="bg-white">Background White Color</div>
```

Eye of a newt, hair of a steer,  
Make this element disappear:
```html
<p class="invisible">Hello</p>
```

### _11. Spacing_

_Note: the margin and padding classes use the notation (property)(sides)-(size), with size being the multiple of a spacer set by Bootstrap_.

Sides values:
* _t_ : top
* _b_ : bottom
* _l_ : left
* _r_ : right
* _x_ : both left and right
* _y_ : both top and bottom
* If no value is specified, all sides are selected

Margin bottom:
```html
<h1 class="mb-0">Margin Bottom 0</h1>
<h1 class="mb-1">Margin Bottom 1</h1>
<h1 class="mb-2">Margin Bottom 2</h1>
<h1 class="mb-3">Margin Bottom 3</h1>
<h1 class="mb-4">Margin Bottom 4</h1>
<h1 class="mb-5">Margin Bottom 5</h1>
```

Margin top:
```html
<h1 class="mt-0">Margin Top 0</h1>
<h1 class="mt-1">Margin Top 1</h1>
<h1 class="mt-2">Margin Top 2</h1>
<h1 class="mt-3">Margin Top 3</h1>
<h1 class="mt-4">Margin Top 4</h1>
<h1 class="mt-5">Margin Top 5</h1>
```

Left and right margins:
```html
<p><span class="mr-5">Margin Right 5</span> dolor sit amet, <span class="ml-3">Margin Left 3 </span> elit. Voluptatum, optio.</p>

<p>Lorem ipsum<span class="mx-5">Margin Left & Right 5</span>, consectetur elit. Voluptatum, optio.</p>
```

Top and bottom margins:
```html
<p>Lorem ipsum dolor sit amet, consectetur elit. Voluptatum, optio.</p>
<p class="my-5">Margin Top & Bottom 5</p>
<p>Lorem ipsum dolor sit amet, consectetur elit. Voluptatum, optio.</p>
```

Margin all sides:
```html
<p>Lorem ipsum dolor sit amet, consectetur elit. Voluptatum, optio.</p>
<p class="m-5">Margin All Sides 5</p>
<p>Lorem ipsum dolor sit amet, consectetur elit. Voluptatum, optio.</p>
```

Padding bottom:
```html
<h1 class="pb-0">Padding Bottom 0</h1>
<h1 class="pb-1">Padding Bottom 1</h1>
<h1 class="pb-2">Padding Bottom 2</h1>
<h1 class="pb-3">Padding Bottom 3</h1>
<h1 class="pb-4">Padding Bottom 4</h1>
<h1 class="pb-5">Padding Bottom 5</h1>
```

Padding top:
```html
<h1 class="pt-0">Padding Top 0</h1>
<h1 class="pt-1">Padding Top 1</h1>
<h1 class="pt-2">Padding Top 2</h1>
<h1 class="pt-3">Padding Top 3</h1>
<h1 class="pt-4">Padding Top 4</h1>
<h1 class="pt-5">Padding Top 5</h1>
```

Left and right padding:
```html
<p><span class="pr-5">Padding Right 5</span> dolor sit amet, <span class="pl-3">Padding Left 3 </span> elit. Voluptatum, optio.</p>

<p>Lorem ipsum<span class="px-5">Padding Left & Right 5</span>, consectetur elit. Voluptatum, optio.</p>
```

Top and bottom padding:
```html
<p class="py-5">Padding Top & Bottom 5</p>
```

Padding all sides:
```html
<p class="p-5">Padding All Sides 5</p>
```

Center align:
```html
<div class="mx-auto" style="width: 200px;">
  Center Align
</div>
```

### _11. Sizing and Borders_

Width classes:
```html
<div class="w-25">Width 25% of container</div>
<div class="w-50">Width 50%</div>
<div class="w-75">Width 75%</div>
<div class="w-100">Width 100%</div>
```
Height classes:
```html
<div class="h-25">Height 25%</div>
<div class="h-50">Height 50%</div>
<div class="h-75">Height 75%</div>
<div class="h-100">Height 100%</div>
```
_Note: While you might think you can swap out other values for the percentage, like w-30 for 30% width or h-60 for 60% height, you can't. Only 25, 50, 75, and 100 are permitted within Bootstrap_.

Border madness:
```html
<div class="bg-light border">Regular</div>
<div class="bg-light border border-primary">Primary</div>
<div class="bg-light border border-secondary rounded">Secondary with rounded borders</div>
<div class="bg-light border border-success rounded-top">Success with borders rounded only on top</div>
<div class="bg-light border border-info rounded-bottom">Info with borders rounded only on the bottom</div>
<div class="bg-light border border-warning rounded-left">Warning with borders rounded only on the left</div>
<div class="bg-light border border-danger border-top-0">Danger with no top border</div>
<div class="bg-light border border-light border-bottom-0">Light with no bottom border</div>
<div class="bg-light border border-dark border-right-0">Dark with no right border</div>
<div class="bg-light border border-white border-left-0">White with no left border</div>
```

### _12. CSS Breakpoints_

```css
// Extra small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// Small devices (landscape phones, 576px and up)
@media (min-width: 576px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... }

// Large devices (desktops, 992px and up)
@media (min-width: 992px) { ... }

// Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```
