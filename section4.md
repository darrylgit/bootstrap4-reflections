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

### _26. Grid Alignment_
```html
<!-- VERTICAL ALIGNMENT -->
<div class="container">
    <div class="row align-items-start" style="height:200px;border:1px #333 solid">
        <div class="col">
            Top Aligned Text (default)
        </div>
        <div class="col">
            Top Aligned Text (default)
        </div>
        <div class="col">
            Top Aligned Text (default)
        </div>
    </div>
    <div class="row align-items-center" style="height:200px;border:1px #333 solid">
        <div class="col">
            Middle Aligned Text
        </div>
        <div class="col">
            Middle Aligned Text
        </div>
        <div class="col">
            Middle Aligned Text
        </div>
    </div>
    <div class="row align-items-end" style="height:200px;border:1px #333 solid">
        <div class="col">
            Bottom Aligned Text
        </div>
        <div class="col">
            Bottom Aligned Text
        </div>
        <div class="col">
            Bottom Aligned Text
        </div>
    </div>
</div>

<br><br>

<!-- VERTICAL ALIGN INDIVIDUAL COLS -->
<div class="container">
    <div class="row" style="height:200px;border:1px #333 solid">
        <div class="col align-self-start">
            Top Aligned (default)
        </div>
        <div class="col align-self-center">
            Middle Aligned
        </div>
        <div class="col align-self-end">
            Bottom Aligned
        </div>
    </div>
</div>

<br><br>

<!-- HORIZONTAL ALIGNED COLS -->
<div class="container">
    <div class="row justify-content-start" style="height:200px;border:1px #333 solid">
        <div class="col-4">
            Left Aligned Text (default)
        </div>
        <div class="col-4">
            Left Aligned Text (default)
        </div>
    </div>
    <div class="row justify-content-center" style="height:200px;border:1px #333 solid">
        <div class="col-4">
            Center Aligned Text
        </div>
        <div class="col-4">
            Center Aligned Text
        </div>
    </div>
    <div class="row justify-content-end" style="height:200px;border:1px #333 solid">
        <div class="col-4">
            Right Aligned Text
        </div>
        <div class="col-4">
            Right Aligned Text
        </div>
    </div>
    <div class="row justify-content-around" style="height:200px;border:1px #333 solid">
        <div class="col-4">
            Content Around
        </div>
        <div class="col-4">
            Content Around
        </div>
    </div>
    <div class="row justify-content-between" style="height:200px;border:1px #333 solid">
        <div class="col-4">
            Content Between
        </div>
        <div class="col-4">
            Content Between
        </div>
    </div>
</div>
```

_Column wrapping_: if the sum of the column values is greater than 12, they automatically wrap  
_no-gutters_: gets rid of the space between columns
```html
<div class="row no-gutters">
    <div class="col-9">
      <div class="card">
        <div class="card-body"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur, repudiandae!</p></div>
      </div>
    </div>
    <div class="col-4">
      <div class="card">
        <div class="card-body"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur, repudiandae!</p></div>
      </div>
    </div>
    <div class="col-6">
      <div class="card">
        <div class="card-bodys"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur, repudiandae!</p></div>
      </div>
    </div>
</div>
</div>
