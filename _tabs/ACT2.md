---
layout: page
icon: fas fa-stream
order: 3
title: "ACT 2 — Creators Response"   # this is used in sidebar             # custom key Chirpy uses to hide top title
---

<!-- ====== Swiper CSS & JS ====== -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

<!-- ====== Carousel container ====== -->
<div class="carousel-wrapper">

  <noscript>
    <div class="js-fallback">
      <img src="/assets/img/FortniteWP.jpg" alt="Fortnite" />
    </div>
  </noscript>

  <div class="swiper mySwiper">
    <div class="swiper-wrapper">

      <div class="swiper-slide">
        <img src="/assets/img_2/slider1.jpg" alt="Fortnite">
      </div>

      <div class="swiper-slide">
        <img src="/assets/img_2/slider2.jpg" alt="PUBG">
      </div>

      <div class="swiper-slide">
        <img src="/assets/img_2/slider3.jpg" alt="Apex Legends">
      </div>

    </div>

    <div class="swiper-pagination"></div>
  </div>

</div>

<!-- ====== Styles ====== -->
<style>
.carousel-wrapper {
  max-width: 980px;
  margin: 0 auto 2rem;
}

.swiper {
  width: 100%;
  padding: 2rem 0;
}

/* Only ONE swiper-slide definition */
.swiper-slide {
  width: 520px;
  height: 290px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  border-radius: 16px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.20);
  background: #0f1720;
}

.swiper-slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.swiper-pagination {
  margin-top: 1rem;
}

/* Responsive */
@media (max-width: 700px) {
  .swiper-slide { width: 86vw; height: 50vw; }
  .carousel-wrapper { padding: 0 1rem; }
}
</style>

<!-- ====== Init script ====== -->
<script>
document.addEventListener('DOMContentLoaded', function () {
  if (typeof Swiper === 'undefined') return;

  new Swiper('.mySwiper', {
    effect: 'coverflow',
    grabCursor: true,
    centeredSlides: true,
    slidesPerView: 'auto',
    loop: false,
    spaceBetween: 16,

    coverflowEffect: {
      rotate: 18,
      stretch: 0,
      depth: 120,
      modifier: 1,
      slideShadows: true
    },

    pagination: {
      el: '.swiper-pagination',
      clickable: true
    }
  });
});
</script>


<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Did posting BR videos accelerate channel growth ?
</h2>

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Did existing creators pivot to BR content ?
</h2>

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Were BR-focused creators more "opportunistic" ?
</h2>

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Did creators abuse BR tags for visibility ?
</h2>

<h2 style="color:#003c9e; font-size:1.5rem; font-weight:900 !important;">
  Did BR introduce new video formats (length, frequency) ?
</h2>
