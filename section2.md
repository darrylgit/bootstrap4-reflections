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
