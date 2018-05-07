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


### _9.Floats and Positions_

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
