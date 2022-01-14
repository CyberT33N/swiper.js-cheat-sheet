# swiper.js Cheat Sheet
Cheat Sheet for swiper.js with the most needed stuff..


# Init swiper

```
// Initialize Swiper
const swiper = new Swiper('.mySwiper', {
        observer: true,
        observeParents: true,
        parallax: true,

        direction: 'horizontal',
        speed: 750,

        // centerInsufficientSlides: true,
        // centeredSlides: true,
        // centeredSlidesBounds: true,

        //
        // slidesOffsetAfter: 500,
        // slidesOffsetBefore: 200,

        dynamicBullets: true,

        keyboard: {
            enabled: true,
            onlyInViewport: true
        },

        effect: 'coverflow',
        coverflowEffect: {
            rotate: 30,
            slideShadows: false,
            // scale: 1.2,
            depth: 400
        },

        pagination: {
            el: '.swiper-pagination',
            clickable: true
        },

        breakpoints: {
            640: {
                slidesPerView: 2,
                spaceBetween: 20,
                grid: { rows: 3 }
            },
            768: {
                slidesPerView: 3,
                spaceBetween: 30,
                grid: { rows: 3 }
            },
            1024: {
                slidesPerView: 3,
                spaceBetween: 0,
                grid: { rows: 3 }
            },
            1280: {
                slidesPerView: 3,
                spaceBetween: 0,
                grid: { rows: 3 }
            }
        },

        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
        }
    })
```












<br><br>
<br><br>
__________________________________________________________

<br><br>
<br><br>


# Check if slide reached last page
```
swiper.on('reachEnd', function(){
     console.log("reach to End");
});
```







<br><br>
<br><br>
__________________________________________________________

<br><br>
<br><br>


# Navigation example 
```html
<!-- Swiper -->
<div class="swiper mySwiper">
  <div class="swiper-wrapper">
<!--    <div class="swiper-slide">Slide 1</div>-->
<!--    <div class="swiper-slide">Slide 2</div>-->
<!--    <div class="swiper-slide">Slide 3</div>-->
<!--    <div class="swiper-slide">Slide 4</div>-->
<!--    <div class="swiper-slide">Slide 5</div>-->
<!--    <div class="swiper-slide">Slide 6</div>-->
<!--    <div class="swiper-slide">Slide 7</div>-->
<!--    <div class="swiper-slide">Slide 8</div>-->
<!--    <div class="swiper-slide">Slide 9</div>-->
  </div>

  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>

  <div class="swiper-pagination"></div>
</div>

```

```javascript
const swiper = new Swiper('.mySwiper', {
        observer: true,
        observeParents: true,
        parallax: true,

        direction: 'horizontal',
        speed: 750,
        
        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev'
        }
    })
```
