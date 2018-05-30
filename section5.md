## Section 5 Reflections

Note: JQuery and Popper.js are required for this section.

### _30. Carousel Slider_
```html
<div class="row">
  <div class="col-sm-8 m-auto">

    <!-- SIMPLE SLIDER -->
    <div id="slider1" class="carousel slide mb-5" data-ride="carousel">
      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
          <img class="d-block img-fluid" src="img/image1.jpg" alt="First Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image2.jpg" alt="Second Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image3.jpg" alt="Third Slide">
        </div>
      </div>
    </div>

    <!-- SLIDER WITH CONTROLS -->
    <div id="slider2" class="carousel slide mb-5" data-ride="carousel">
      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
          <img class="d-block img-fluid" src="img/image1.jpg" alt="First Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image2.jpg" alt="Second Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image3.jpg" alt="Third Slide">
        </div>
      </div>
      <a href="#slider2" class="carousel-control-prev" data-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </a>
      <a href="#slider2" class="carousel-control-next" data-slide="next">
        <span class="carousel-control-next-icon"></span>
      </a>
    </div>
    <!-- SLIDER WITH INDICATORS -->
    <div id="slider3" class="carousel slide mb-5" data-ride="carousel">
      <ol class="carousel-indicators">
        <li class="active" data-target="#slider3" data-slide-to="0"></li>
        <li data-target="#slider3" data-slide-to="1"></li>
        <li data-target="#slider3" data-slide-to="2"></li>
      </ol>
      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
          <img class="d-block img-fluid" src="img/image1.jpg" alt="First Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image2.jpg" alt="Second Slide">
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image3.jpg" alt="Third Slide">
        </div>
      </div>
      <a href="#slider3" class="carousel-control-prev" data-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </a>
      <a href="#slider3" class="carousel-control-next" data-slide="next">
        <span class="carousel-control-next-icon"></span>
      </a>
    </div>
    <!-- SLIDER WITH CAPTIONS -->
    <div id="slider4" class="carousel slide mb-5" data-ride="carousel">
      <ol class="carousel-indicators">
        <li class="active" data-target="#slider4" data-slide-to="0"></li>
        <li data-target="#slider4" data-slide-to="1"></li>
        <li data-target="#slider4" data-slide-to="2"></li>
      </ol>
      <div class="carousel-inner" role="listbox">
        <div class="carousel-item active">
          <img class="d-block img-fluid" src="img/image1.jpg" alt="First Slide">
          <div class="carousel-caption d-none d-md-block">
            <h3>Slide One</h3>
            <p>Lorem ipsum dolor sit amet, consectetur.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image2.jpg" alt="Second Slide">
          <div class="carousel-caption d-none d-md-block">
            <h3>Slide Two</h3>
            <p>Lorem ipsum dolor sit amet, consectetur.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img class="d-block img-fluid" src="img/image3.jpg" alt="Third Slide">
          <div class="carousel-caption d-none d-md-block">
            <h3>Slide Three</h3>
            <p>Lorem ipsum dolor sit amet, consectetur.</p>
          </div>
        </div>
      </div>
      <a href="#slider4" class="carousel-control-prev" data-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </a>
      <a href="#slider4" class="carousel-control-next" data-slide="next">
        <span class="carousel-control-next-icon"></span>
      </a>
    </div>
  </div>
</div>
```

We can also edit the carousel object and add event handlers on and after the slide:
```javascript
$('.carousel').carousel({
  interval:3000,
  keyboard: true,
  pause: 'hover',
  wrap: true //if false, slider stops at the last slide
});

$('#slider4').on('slide.bs.carousel', function() {
  console.log('slide')
})

$('#slider4').on('slid.bs.carousel', function() {
  console.log('slid')
})
```
