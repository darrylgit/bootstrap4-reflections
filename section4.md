## Section 4 Reflections

### _26. Grid System_
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

### _27. Grid Alignment_
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
```

### _28. Flexbox_
```html
<!-- FLEX ROW & FLEX ITEMS -->
<div class="d-flex flex-row">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- FLEX ROW REVERSE -->
<div class="d-flex flex-row-reverse">
  <div class="p-4">Flex Item starting from the right</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- JUSTIFY CONTENT -->
<!-- Justify left (default)-->
<div class="d-flex flex-row justify-content-start">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- Justify center -->
<div class="d-flex flex-row justify-content-center">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- Justify right -->
<div class="d-flex flex-row justify-content-end">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- Justify with space around items -->
<div class="d-flex flex-row justify-content-around">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- Justify with space between items-->
<div class="d-flex flex-row justify-content-between">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- FLEX CONTAINER / FLEX COLUMN -->
<div class="d-flex flex-column">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<div class="d-flex flex-column reverse">
  <div class="p-4">Flex Item from the bottom</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- VERTICAL ALIGN ITEMS -->
<div class="d-flex flex-row align-items-start">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- VERTICAL ALIGN ITEMS -->
<div class="d-flex flex-row align-items-center">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- VERTICAL ALIGN ITEMS -->
<div class="d-flex flex-row align-items-end">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- VERTICAL ALIGN ITEMS -->
<div class="d-flex flex-row align-items-baseline">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- VERTICAL ALIGN ITEMS -->
<div class="d-flex flex-row align-items-stretch">
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
  <div class="p-4">Flex Item</div>
</div>

<br><br>

<!-- ALIGN SELF -->
<div class="d-flex flew-row">
  <div class="p-4 align-self-start">Flex Item</div>
  <div class="p-4 align-self-center">Flex Item</div>
  <div class="p-4 align-self-end">Flex Item</div>
  <div class="p-4 align-self-baseline">Flex Item</div>
  <div class="p-4 align-self-stretch">Flex Item</div>
</div>

<br><br>

<!-- RESPONSIVE ALIGN SELF -->
<div class="d-flex flew-row">
  <div class="p-4 align-self-md-start">Flex Item</div>
  <div class="p-4 align-self-md-center">Flex Item</div>
  <div class="p-4 align-self-md-end">Flex Item</div>
  <div class="p-4 align-self-md-baseline">Flex Item</div>
  <div class="p-4 align-self-md-stretch">Flex Item</div>
</div>
```

### _29. Auto Margin, Wrap, and Ordering_
```html
<!-- MR-AUTO (last two items get pushed to right) -->
<div class="d-flex row-hl">
    <div class="mr-auto p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
</div>

<br><br>

<!-- ML-AUTO (first two items get pushed to left) -->
<div class="d-flex row-hl">
    <div class="p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
    <div class="ml-auto p-2 item-hl">Flex item</div>
</div>

<br><br>

<!-- MB-AUTO (last two items get pushed to bottom) -->
<div class="d-flex flex-column row-hl">
    <div class="mb-auto p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
</div>

<br><br>

<!-- MT-AUTO (first two items get pushed to top) -->
<div class="d-flex flex-column row-hl">
    <div class="p-2 item-hl">Flex item</div>
    <div class="p-2 item-hl">Flex item</div>
    <div class="mt-auto p-2 item-hl">Flex item</div>
</div>

<br><br>

<!-- NO WRAP -->
<div class="d-flex no-wrap row-hl">
  <div> a number of flex items </div>
</div>

<br><br>

<!-- WRAP -->
<div class="d-flex flex-wrap row-hl">
  <div> a number of flex items </div>
</div>

<br><br>

<!-- ORDERING -->
<div class="d-flex row-hl">
  <div class="order-3 p-2 item-hl">First flex item</div>
  <div class="order-2 p-2 item-hl">Second flex item</div>
  <div class="order-1 p-2 item-hl">Third flex item</div>
</div>
```
