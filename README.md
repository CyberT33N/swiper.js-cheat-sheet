# swiper.js Cheat Sheet
Cheat Sheet for swiper.js with the most needed stuff..


# Init swiper

```
// Initialize Swiper
const swiper = new Swiper('.mySwiper', {
    // centerInsufficientSlides: true,
    // centeredSlides: true,
    // centeredSlidesBounds: true,

     //
     // slidesOffsetAfter: 500,
     // slidesOffsetBefore: 200,

    keyboard: {
        enabled: true,
        onlyInViewport: true,
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

    navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
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
    }
})
```



<br><br>
<br><br>


# Check if slide reached last page
```
swiper.on('reachEnd', function(){
     console.log("reach to End");
});
```
