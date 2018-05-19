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

### _16. Navabars & Navs_

Simple navbar:
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
          <ul class="navbar-nav">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
      </div>
</nav>
```
_Explanation of classes_:  
* _bg-light_: Can be swapped out for any bootstrap color, (eg. _bg-primary_, _bg-danger_, and _bg-success_).
* _navbar-light_: Should correspond to the background. _navbar-light_ will make your text readable on a light background, and _navbar-dark_ will make your text readable on a dark background.
* _navbar-brand_: The name of the website or page, separate from clickable nav items
* _navbar-expand-sm_: When the screen width hits the sm (small) mark, the nav items responsively lose their inline properties and become a vertical list to save space.


But what if you don't want a vertical list? What about a responsive toggle?
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler"
      data-toggle="collapse"
      data-target="#navbarNav"><span
      class="navbar-toggler-icon"></span></button>
          <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ml-auto">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
        </div>
      </div>
</nav>
```

Navbar with form (and responsive toggle):
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler"
      data-toggle="collapse"
      data-target="#navbarNav"><span
      class="navbar-toggler-icon"></span></button>
          <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav mr-auto">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>

          <form class="form-inline my-2 my-lg-0">
            <input  type="text" class="form-control mr-sm-2"
            placeholder="Search">
            <button class="btn btn-outline-success my-2 my-sm-0">Search</button>
          </form>
        </div>
      </div>
</nav>
```

Navbar with dropdown:
```html
<nav class="navbar navbar-expand-sm navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Navbar</a>
          <ul class="navbar-nav">
              <li class="nav-item">
                  <a class="nav-link" href="#">Home</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" data-toggle="dropdown">Dropdown</a>
                <div class="dropdown-menu">
                  <a href="#" class="dropdown-item">Link 1</a>
                  <a href="#" class="dropdown-item">Link 2</a>
                  <a href="#" class="dropdown-item">Link 3</a>
                </div>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                  <a class="nav-link" href="#">Contact</a>
              </li>
          </ul>
      </div>
</nav>
```

Navs (essentially navbars with no background):
```html
<ul class="nav">
    <li class="nav-item">
        <a class="nav-link" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```

Highlight active elements with _nav-pills_:
```html
<ul class="nav nav-pills">
    <li class="nav-item">
        <a class="nav-link active" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```

_ul_ positioning classes for navs:   
* _justify-content-center_: Center align
* _justify-content-end_: Right align
* _flex-column_: A column
* _nav-fill_: Makes the nav a block and gives each item an equal fill


Nav with dropdown:
```html
<ul class="nav nav-fill">
    <li class="nav-item">
        <a class="nav-link" href="#">Link 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 2</a>
    </li>
    <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle"
        href="#" data-toggle="dropdown">Dropdown</a>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Link 1</a>
          <a class="dropdown-item" href="#">Link 2</a>
          <a class="dropdown-item" href="#">Link 3</a>
        </div>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link" href="#">Link 4</a>
    </li>
</ul>
```

### _17. List Groups and Badges_

Basic list group:
```html
<ul class="list-group">
    <li class="list-group-item">My List Item One</li>
    <li class="list-group-item">My List Item Two</li>
    <li class="list-group-item">My List Item Three</li>
    <li class="list-group-item">My List Item Four</li>
    <li class="list-group-item">My List Item Five</li>
</ul>
```

List group with hoverable links:
```html
<ul class="list-group">
    <a class="list-group-item list-group-item-action" href="#">My List Item One</a>
    <a class="list-group-item list-group-item-action" href="#">My List Item Two</a>
    <a class="list-group-item list-group-item-action" href="#">My List Item Three</a>
    <a class="list-group-item list-group-item-action" href="#">My List Item Four</a>
    <a class="list-group-item list-group-item-action" href="#">My List Item Five</a>
</ul>
```

Pretty colors:
```html
<ul class="list-group">
    <li class="list-group-item">Regular List Item</li>
    <li class="list-group-item list-group-item-primary">Primary List Item</li>
    <li class="list-group-item list-group-item-secondary">Secondary List Item</li>
    <li class="list-group-item list-group-item-success">Success List Item</li>
    <li class="list-group-item list-group-item-info">Info List Item</li>
    <li class="list-group-item list-group-item-warning">Warning List Item</li>
    <li class="list-group-item list-group-item-danger">Danger List Item</li>
    <li class="list-group-item list-group-item-light">Light List Item</li>
    <li class="list-group-item list-group-item-dark">Dark List Item</li>
</ul>
```

A Javascript list widget _(note: requires JQuery and Popper.js)_:
```html
<div class="row mb-5">
  <div class="col-4">
    <div class="list-group" id="list-tab" role="tablist">
        <a class="list-group-item list-group-item-action active" id="list-home-list"
        href="#list-home" data-toggle="list">Home</a>
        <a class="list-group-item list-group-item-action" id="list-about-list"
        href="#list-about" data-toggle="list">About</a>
        <a class="list-group-item list-group-item-action" id="list-services-list"
        href="#list-services" data-toggle="list">Services</a>
    </div>
  </div>
  <div class="col-8">
    <div class="tab-content" id="nav-tabContent">
      <div class="tab-pane fade show active" id="list-home" role="tabpanel">
        Home Content...
      </div>
      <div class="tab-pane fade" id="list-about" role="tabpanel">
        About Content...
      </div>
      <div class="tab-pane fade" id="list-services" role="tabpanel">
        Services Content...
      </div>
    </div>
  </div>
</div>
```

Badges:
```html
<ul class="list-group">
    <li class="list-group-item">My List Item One</li>
    <li class="list-group-item d-flex justify-content-between
    align-items center">My List Item Two <span class="badge badge-primary">30</span></li>
    <li class="list-group-item">My List Item Three</li>
    <li class="list-group-item">My List Item Four</li>
    <li class="list-group-item">My List Item Five</li>
</ul>
```

Breadcrumbs:
```html
<ol class="breadcrumb">
    <li class="breadcrumb-item active">Home</li>
</ol>
<ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item active">Users</li>
</ol>
<ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Users</a></li>
    <li class="breadcrumb-item active">Brad</li>
</ol>
```

### _18. Forms & Input_

Form madness:
```html
<form>
    <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" class="form-control form-control-sm" placeholder="Enter name">
    </div>
    <div>
        <label for="email">Email address</label>
        <input type="email" id="email" class="form-control form-control-lg" placeholder="Enter email">
        <small class="form-text text-muted">Your email will not be shared with anyone</small>
    </div>
    <div class="form-group">
         <label for="password">Password</label>
        <input type="password" id="password" class="form-control" placeholder="Password" readonly>
    </div>
    <div class="form-group">
        <label for="gender">Gender</label>
        <select id="gender" class="form-control">
        <option>Male</option>
        <option>Female</option>
        </select>
    </div>
    <div class="form-group">
        <label for="message">Message</label>
        <textarea id="message" class="form-control" rows="3"></textarea>
    </div>
    <div class="form-group">
        <label for="file">File input</label>
        <input type="file" id="file" class="form-control-file">
        <small id="fileHelp" class="form-text text-muted">Max 3mb size</small>
    </div>
```
Explanation of classes:  
* _form-group_: Adds margins
* _form-control_: Makes the input a block-level element, rounds corners
* _form-control-file_: Specifically for file inputs
* _form-text_: Adjusts margins


Form checks:
```html
<fieldset class="form-group">
    <legend>What are you using this service for?</legend>
    <div class="form-check">
      <label class="form-check-label">
          <input type="radio" value="option1" class="form-check-input" checked>
          Personal
      </label>
    </div>
    <div class="form-check">
      <label class="form-check-label">
          <input type="radio" value="option1" class="form-check-input" checked>
          Commercial Use
      </label>
    </div>
    <div class="form-check">
      <label class="form-check-label">
          <input type="radio" value="option1" class="form-check-input" checked>
          Testing
      </label>
    </div>
</fieldset>
<div class="form-check">
    <label class="form-check-label">
    <input type="checkbox" class="form-check-input">
        Sign up for newsletter
    </label>
</div>
<button class="btn btn-primary" type="submit">Submit</button>
</form>
```

Inline forms:
```html
<form class="form-inline">
    <input type="text" class="form-control mr-2" id="username" placeholder="Enter username">
    <input type="text" class="form-control mr-2" id="password" placeholder="Password">
    <div class="form-check">
        <label class="form-check-label mr-2">
            <input type="checkbox" class="form-check-input"> Remember me
        </label>
    </div>

    <button type="submit" class="btn btn-secondary">Submit</button>
</form>
```

Form row:
```html
<form>
  <div class="form-row">
    <div class="col">
      <input type="text" class="form-control" placeholder="First name">
    </div>
    <div class="col">
      <input type="text" class="form-control" placeholder="Last name">
    </div>
  </div>
</form>
```

Validation:
```html
<div class="form-group">
    <label for="username">Username</label>
    <input type="text" id="username" class="form-control is-valid">
</div>
<div class="form-group">
    <label for="password">Password</label>
    <input type="text" id="password" class="form-control is-invalid">
    <div class="invalid-feedback">
      Password not strong enough
    </div>
</div>
<div class="form-group">
    <label for="password2">Confirm Password</label>
    <input type="text" id="password2" class="form-control is-invalid">
    <div class="invalid-feedback">
      Password does not match
    </div>
</div>
```
Explanation of classes:  
* _is-valid_: Makes border green
* _is-invalid_: Makes border red
* _invalid-feedback_: Makes text red

### _19. Input Groups & Addons_

Simple input groups with addons:
```html
<div class="input-group">
    <span class="input-group-addon">@</span>
    <input type="text" class="form-control" placeholder="Username">
</div>
<br>
<div class="input-group">
    <input type="text" class="form-control" placeholder="Email address">
    <span class="input-group-addon">@something.com</span>
</div>
<br>
<label for="profile-url">Choose profile URL</label>
<div class="input-group">
    <span class="input-group-addon">https://something.com/member/</span>
    <input type="text" class="forn-control" id="profile-url">
</div>
<br>
<div class="input-group">
    <span class="input-group-addon">$</span>
    <input type="text" class="form-control">
    <span class="input-group-addon">.00</span>
</div>
```

Large input group:
```html
<div class="input-group input-group-lg">
    <span class="input-group-addon">@</span>
    <input type="text" placeholder="Username" class="form-control">
</div>
```

Input groups with checks:
```html
<div class="input-group">
    <span  class="input-group-addon">
        <input type="checkbox">
    </span>
    <input type="text" class="form-control">
</div>
<br>
<div class="input-group">
    <span class="input-group-addon">
        <input type="radio">
    </span>
    <span class="input-group-addon">$5.00</span>
    <input type="text" class="form-control">
</div>
```

Input group with button:
```html
<div class=input-group>
   <input type="text" class="form-control" placeholder="Search for...">
   <span class="input-group-btn">
       <button class="btn btn-primary" type="button">Search</button>
   </span>
</div>
```

### _20. Alerts and Progress Bars_

Alerts:
```html
<div class="alert alert-primary">
  <strong>Primary</strong> Blog post added
</div>

<div class="alert alert-secondary">
  <strong>Secondary</strong> Blog post added
</div>

<div class="alert alert-success">
    <strong>Success</strong> Blog post added
</div>

<div class="alert alert-danger">
    <strong>Danger</strong> Please check the log files
</div>

<div class="alert alert-info">
    <strong>Info</strong> You have a new message
</div>

<div class="alert alert-warning">
    <strong>Warning</strong> Please check the log files
</div>

<div class="alert alert-light">
    <strong>Light</strong> Please check the log files <a class="alert-link">Read more</a>
</div>

<div class="alert alert-dark">
    <strong>Dark</strong> Please check the log files
</div>

<!-- DISMISSABLE ALERT -->
<div class="alert alert-success alert-dismissable fade show">
    <button class="close" data-dismiss="alert" type="button">
        <span>&times;</span>
    </button>
    <strong>Dismissable</strong> Blog post added
</div>
```

Progress bars:
```html
<div class="progress">
    <div class="progress-bar" style="width:35%;"></div>
</div>
<br>
<div class="progress">
    <div class="progress-bar" style="width:35%;">35%</div>
</div>
<br>
<div class="progress">
    <div class="progress-bar bg-success" style="width:45%;"></div>
</div>
<br>
<div class="progress">
    <div class="progress-bar bg-info" style="width:55%;"></div>
</div>
<br>
<div class="progress">
    <div class="progress-bar bg-warning" style="width:85%;"></div>
</div>
<br>
<div class="progress">
    <div class="progress-bar bg-danger progress-bar-striped" style="width:85%;"></div>
</div>
<br>
<div class="progress">
    <div class="progress-bar bg-danger progress-bar-striped
    progress-bar-animated" style="width:85%;"></div>
</div>
```

### _21. Tables and Pagination_

Tables:
```html
<!-- BASIC TABLE -->
<table class="table">
    <thead>
        <tr>
            <th>#</th>
            <th>First Name</th>
            <th>Last Name</th>
            <th>Email</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope="row">1</th>
            <td>John</td>
            <td>Doe</td>
            <td>jdoe@gmail.com</td>
        </tr>
        <tr>
            <th scope="row">2</th>
            <td>Will</td>
            <td>Johnson</td>
            <td>will@yahoo.com</td>
        </tr>
        <tr>
            <th scope="row">3</th>
            <td>Shannon</td>
            <td>Williams</td>
            <td>shannon@yahoo.com</td>
        </tr>
    </tbody>
</table>

<!-- INVERSE (dark) TABLE -->
<table class="table table-inverse">


<!-- TABLE HEAD INVERSE (dark) -->
<table class="table">
    <thead class="thead-inverse">


<!-- STRIPED TABLE -->
<table class="table table-striped">


<!-- BORDERED TABLE -->
<table class="table table-bordered">


<!-- HOVERABLE -->
<table class="table table-hover">


<!-- SMALL TABLE -->
<table class="table table-sm">
```

Pagination:
```html
<!-- BASIC -->
<nav>
    <ul class="pagination">
        <li class="page-item disabled"><a class="page-link" href="#">Previous</a></li>
        <li class="page-item active"><a class="page-link" href="#">1</a></li>
        <li class="page-item"><a class="page-link" href="#">2</a></li>
        <li class="page-item"><a class="page-link" href="#">3</a></li>
        <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>
</nav>

<!-- PAGINATION CENTERED -->
<nav>
    <ul class="pagination justify-content-center">
    </ul>
</nav>


<!-- PAGINATION RIGHT -->
<nav>
    <ul class="pagination justify-content-end">
    </ul>
</nav>

<!-- PAGINATION LARGE -->
<nav>
    <ul class="pagination pagination-lg">
    </ul>
</nav>


<!-- PAGINATION SMALL -->
<nav>
    <ul class="pagination pagination-sm">
    </ul>
</nav>
```

### _22. Cards_
```html
<!-- SIMPLE CARD -->
<div class="card">
    <div class="card-body">
        <h4 class="card-title">Card Title</h4>
        <h6 class="card-subtitle">Card subtitle</h6>
        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo, quas.</p>
         <a href="#" class="btn btn-outline-primary">Read More</a>
    </div>
</div>

<br><br>

<!-- CARD WITH IMAGE -->
<div class="card" style="width:20rem">
    <img class="card-img-top" src="http://lorempixel.com/300/300/sports/" alt="Card image cap">
    <div class="card-body">
        <h4 class="card-title">Card Title</h4>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Illo, quas.</p>
         <a class="btn btn-success btn-block" href="#">Read More</a>
    </div>
</div>

<br><br>

<!-- HEADER, FOOTER, CENTERED -->
<div class="card text-center">
    <div class="card-header">
        My Card
    </div>
    <div class="card-body">
        <h4 class="card-title">Card Title</h4>
        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut, perspiciatis.</p>
        <a href="#" class="btn btn-danger">Read More</a>
    </div>
    <div class="card-footer text-muted">
      2 Days Ago
    </div>
</div>

<br><br>

<!-- CARD WITH NAV -->
<div class="card">
    <div class="card-header">
        <ul class="nav nav-tabs card-header-tabs">
        <li class="nav-item">
            <a class="nav-link active" href="#">Active</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="#">Disabled</a>
        </li>
        </ul>
    </div>
    <div class="card-body">
        <h4 class="card-title">Card Title</h4>
        <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aut, perspiciatis.</p>
        <a class="btn btn-primary" href="#">Read More</a>
    </div>
</div>

<br><br>

<!-- IMAGE OVERLAYS -->
<div class="card bg-dark text-white">
    <img class="card-img" src="http://lorempixel.com/900/200/sports/">
    <div class="card-img-overlay">
        <h4 class='card-title'>Card title</h4>
        <p class="card-text">This is a wider card with supporting text below as
          a natural lead-in to additional content. This content is a little bit
          longer.</p>
        <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small>
        </p>
    </div>
</div>

<br><br>

<!-- BACKGROUND COLOR -->
<div class="card text-white bg-primary mb-3">
  <div class="card-header">Header</div>
  <div class="card-body">
    <h4 class="card-title">Primary card title</h4>
    <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing
      elit, sed do eiusmod</p>
  </div>
</div>

<br><br>

<!-- CARD OUTLINE -->
<div class="card border-primary mb-3">
  <div class="card-header">Header</div>
  <div class="card-body">
    <h4 class="card-title">Primary card title</h4>
    <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing
      elit, sed do eiusmod</p>
  </div>
</div>

<br></br>

<!-- CARD GROUP -->
<div class="card-group">
    <div class="card">
        <div class="card-body">
            <h4 class="card-title">Card Title</h4>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur
              adipisicing elit. Illo, quas.</p>
        </div>
    </div>
    <div class="card">
        <div class="card-body">
            <h4 class="card-title">Card Title</h4>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur
              adipisicing elit. Illo, quas.</p>
        </div>
    </div>
    <div class="card">
        <div class="card-body">
            <h4 class="card-title">Card Title</h4>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur
              adipisicing elit. Illo, quas.</p>
        </div>
    </div>
</div>

<br><br>

 <!-- CARD DECK -->
 <div class="card-deck">
     <div class="card">
         <div class="card-body">
             <h4 class="card-title">Card Title</h4>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur
               adipisicing elit. Illo, quas.</p>
         </div>
     </div>
     <div class="card">
         <div class="card-body">
             <h4 class="card-title">Card Title</h4>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur
               adipisicing elit. Illo, quas.</p>
         </div>
     </div>
     <div class="card">
         <div class="card-body">
             <h4 class="card-title">Card Title</h4>
             <p class="card-text">Lorem ipsum dolor sit amet, consectetur
               adipisicing elit. Illo, quas.</p>
         </div>
     </div>
 </div>

<br><br>

<!-- CARD COLUMNS -->
<div class="card-columns">
    <div class="card">
        <img class="card-img-top img-fluid" src="http://lorempixel.com/400/200/sports/1"
        alt="Card image cap">
        <div class="card-body">
          <h4 class="card-title">Card title that wraps to a new line</h4>
          <p class="card-text">This is a longer card with supporting text below
            as a natural lead-in to additional content. This content is a little
            bit longer.</p>
        </div>
    </div>
    <div class="card p-3">
        <blockquote class="card-body card-bodyquote">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer
          posuere erat a ante.</p>
        <footer>
            <small class="text-muted">
            Someone famous in <cite title="Source Title">Source Title</cite>
            </small>
        </footer>
        </blockquote>
    </div>
    <div class="card">
        <img class="card-img-top img-fluid" src="http://lorempixel.com/400/200/sports/2" alt="Card image cap">
        <div class="card-body">
          <h4 class="card-title">Card title</h4>
          <p class="card-text">This card has supporting text below as a natural
            lead-in to additional content.</p>
          <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small>
          </p>
        </div>
    </div>
    <div class="card card-inverse card-primary p-3 text-center">
        <blockquote class="card-bodyquote">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat.</p>
        <footer>
            <small>
            Someone famous in <cite title="Source Title">Source Title</cite>
            </small>
        </footer>
        </blockquote>
    </div>
    <div class="card text-center">
        <div class="card-body">
          <h4 class="card-title">Card title</h4>
          <p class="card-text">This card has supporting text below as a natural
            lead-in to additional content.</p>
          <p class="card-text"><small class="text-muteds">Last updated 3 mins ago</small>
          </p>
        </div>
    </div>
    <div class="card">
        <img class="card-img img-fluid" src="http://lorempixel.com/400/200/sports/3"
        alt="Card image">
    </div>
    <div class="card p-3 text-right">
        <blockquote class="card-bodyquote">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
        <footer>
            <small class="text-muted">
            Someone famous in <cite title="Source Title">Source Title</cite>
            </small>
        </footer>
        </blockquote>
    </div>
    <div class="card">
        <div class="card-body">
          <h4 class="card-title">Card title</h4>
          <p class="card-text">This is a wider card with supporting text below as
            a natural lead-in to additional content. This card has even longer
            content than the first to show that equal height action.</p>
          <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
        </div>
    </div>
</div>
```
