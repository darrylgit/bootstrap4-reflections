## Section 3 Reflections

### _15. Buttons and Button Groups_

Buttons:
```html
<button class="btn btn-primary" type="button">Primary</button>
<button class="btn btn-secondary" type="button">Secondary</button>
<button class="btn btn-success" type="button">Success</button>
<button class="btn btn-info" type="button">Info</button>
<button class="btn btn-warning" type="button">Warning</button>
<button class="btn btn-danger" type="button">Danger</button>
<button class="btn btn-light" type="button">Light</button>
<button class="btn btn-dark" type="button">Dark</button>
<button class="btn btn-link">a button that looks like a link</button>
```

We can add 'btn' classes to:
```html
<a class="btn" href="#" role="button">Link</a>
<button class="btn" type="submit">Button</button>
<input class="btn" type="button" value="Input">
<input class="btn" type="submit" value="Submit">
<input class="btn" type="reset" value="Reset">
```

Outline buttons:
```html
<button class="btn btn-outline-primary" type="button">Primary Outline</button>
<button class="btn btn-outline-secondary" type="button">Secondary Outline</button>
<button class="btn btn-outline-success" type="button">Success Outline</button>
<button class="btn btn-outline-info" type="button">Info Outline</button>
<button class="btn btn-outline-warning" type="button">Warning Outline</button>
<button class="btn btn-outline-danger" type="button">Danger Outline</button>
<button class="btn btn-outline-light" type="button">Light Outline</button>
<button class="btn btn-outline-dark" type="button">Dark Outline</button>
```

Button sizes:
```html
<button class="btn btn-lg" type="button">Large button</button>
<button class="btn btn-sm" type="button">Small button</button>
<button class="btn btn-block" type="button">Block level button</button>
```

Button states:
```html
<button class="btn" type="button">Regular Button</button>
<button class="btn active" type="button">Active Button</button>
<button class="btn disabled" type="button">Disabled Button</button>
<button class="btn" type="button" data-toggle="button">
    Toggle State - the button toggles between regular and active colors when clicked
</button>
```

Button dropdowns:
```html
<div class="dropdown">
    <button class="btn dropdown-toggle" type="button"
    data-toggle="dropdown">
        My Dropdown
    </button>
    <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link One</a>
        <a class="dropdown-item" href="#">Link Two</a>
        <a class="dropdown-item" href="#">Link Three</a>
    </div>
</div>
```

Split dropdowns:
```html
<div class="btn-group">
    <button class="btn" type="button">My Button</button>
    <button class="btn dropdown-toggle" type="button"
    data-toggle="dropdown">
        <span>Toggle Dropdown</span>
    </button>
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Link One</a>
      <a class="dropdown-item" href="#">Link Two</a>
      <a class="dropdown-item" href="#">Link Three</a>
      <div class="dropdown-divider"></div>
      <a class="dropdown-item" href="#">Link Four</a>
    </div>
</div>
```

Button groups:
```html
<div class="btn-group">
    <button class="btn" type="button">Left</button>
    <button class="btn" type="button">Middle</button>
    <button class="btn" type="button">Right</button>
</div>
```

Button toolbar:
```html
<div class="btn-toolbar">
    <div class="btn-group mr-2">
        <button class="btn" type="button">1</button>
        <button class="btn" type="button">2</button>
        <button class="btn" type="button">3</button>
        <button class="btn" type="button">4</button>
    </div>
    <div class="btn-group mr-2">
        <button class="btn" type="button">5</button>
        <button class="btn" type="button">6</button>
        <button class="btn" type="button">7</button>
    </div>
    <div class="btn-group">
        <button class="btn" type="button">8</button>
    </div>
</div>
```

Vertical button groups:
```html
<div class="btn-group-vertical">
    <button class="btn" type="button">Left</button>
    <button class="btn" type="button">Middle</button>
    <button class="btn" type="button">Right</button>
</div>
```
