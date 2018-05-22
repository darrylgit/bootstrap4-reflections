## Section 4 Reflections

### _25. Grid System_
```html
<!-- RESPONSIVE GRID -->
<div class="row">
  <div class="col-sm-6 col-md-8 col-lg-9 col-xl-10" style="border:1px solid #333">
    <ul>
      <li>6 column on small screens</li>
      <li>8 column on medium screens</li>
      <li>9 column on large screens</li>
      <li>10 column on XL screens</li>
      <li>Its own row on extra small screens</li>
    </ul>
  </div>
  <div class="col-sm-6 col-md-4 col-lg-3 col-xl-2" style="border:1px solid #333">
    <ul>
      <li>6 column on small screens</li>
      <li>4 column on medium screens</li>
      <li>3 column on large screens</li>
      <li>2 column on XL screens</li>
      <li>Its own row on extra small screens</li>
    </ul>
  </div>
</div>

<!-- EQUAL WIDTH -->
<div class="row">
  <div class="col" style="border:1px solid #333">Equal Width</div>
  <div class="col" style="border:1px solid #333">Equal Width</div>
  <div class="col" style="border:1px solid #333">Equal Width</div>
</div>

<!-- EQUAL WIDTH MULTI ROW -->
<div class="row">
  <div class="col" style="border:1px solid #333">Equal Width Multi</div>
  <div class="col" style="border:1px solid #333">Equal Width Multi</div>
  <div class="w-100" style="border:1px solid #333"></div>
  <div class="col" style="border:1px solid #333">Equal Width Multi</div>
  <div class="col" style="border:1px solid #333">Equal Width Multi</div>
</div>

<!-- AUTO LAYOUT -->
<div class="row">
  <div class="col" style="border:1px solid #333">Auto Layout</div>
  <div class="col-6" style="border:1px solid #333">Auto Layout</div>
  <div class="col" style="border:1px solid #333">Auto Layout</div>
</div>

<!-- EQUAL WIDTH STACKED (on small screens) -->
<div class="row">
  <div class="col-sm" style="border:1px solid #333">Equal Width Stack</div>
  <div class="col-sm" style="border:1px solid #333">Equal Width Stack</div>
  <div class="col-sm" style="border:1px solid #333">Equal Width Stack</div>
</div>

<!-- ORDERING -->
<div class="row">
  <div class="col order-3" style="border:1px solid #333">
    First
  </div>
  <div class="col order-2" style="border:1px solid #333">
    Second
  </div>
  <div class="col order-1" style="border:1px solid #333">
    Third
  </div>
</div>

<!-- OFFSETTING -->
<div class="row">
  <div class="col-md-4" style="border:1px solid #333">4 col</div>
  <div class="col-md-4 ml-auto" style="border:1px solid #333">4 col offset 4</div>
</div>
<div class="row">
  <div class="col-md-3 ml-auto" style="border:1px solid #333">3 col offset 3</div>
  <div class="col-md-3 ml-auto" style="border:1px solid #333">3 col offset 3</div>
</div>
<div class="row">
  <div class="col-md-6 m-auto" style="border:1px solid #333">6 col offset 3</div>
</div>

<!-- NESTING -->
<div class="row">
  <div class="col-sm-9" style="border:1px solid #333">
    Level 1: .col-sm-9
    <div class="row">
      <div class="col-sm-6" style="border:1px solid red">
        Level 2: .col-8 .col-sm-6
      </div>
      <div class="col-sm-6" style="border:1px solid red">
        Level 2: .col-4 .col-sm-6
      </div>
    </div>
  </div>
</div>
```
