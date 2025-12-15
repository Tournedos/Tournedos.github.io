---
layout: page
icon: fas fa-stream
order: 3
title: "ACT 2 — Creators Response"   # this is used in sidebar             # custom key Chirpy uses to hide top title
---

<!-- ====== Swiper CSS & JS ====== -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

<!-- ====== IMAGES SLIDER ====== -->
<div class="carousel-wrapper">
  <div class="swiper imagesSwiper">
    <div class="swiper-wrapper">

      <div class="swiper-slide">
        <img src="/assets/img/img_2/slider1.jpg" alt="Fortnite">
      </div>

      <div class="swiper-slide">
        <img src="/assets/img/img_2/slider2.jpg" alt="PUBG">
      </div>

      <div class="swiper-slide">
        <img src="/assets/img/img_2/slider3.jpg" alt="Apex Legends">
      </div>

    </div>
    <div class="swiper-pagination"></div>
  </div>
</div>

<!-- ====== FIGURES SLIDER ====== -->
<div class="carousel-wrapper">
  <div class="swiper figuresSwiper">
    <div class="swiper-wrapper">

      <div class="swiper-slide">
        <iframe src="/assets/plots/plots_2/figure_1_1.html" class="figure-frame"></iframe>
      </div>

      <div class="swiper-slide">
        <iframe src="/assets/plots/plots_2/figure_1_2.html" class="figure-frame"></iframe>
      </div>

      <div class="swiper-slide">
        <iframe src="/assets/plots/plots_2/figure_1_3.html" class="figure-frame"></iframe>
      </div>

      <div class="swiper-slide">
        <iframe src="/assets/plots/plots_2/figure_1_4.html" class="figure-frame"></iframe>
      </div>

      <div class="swiper-slide">
        <iframe src="/assets/plots/plots_2/figure_1_5.html" class="figure-frame"></iframe>
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

.swiper-slide {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #0f1720;
}

.swiper-slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 16px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.2);
}

.figure-frame {
  width: 100%;
  height: 600px;  /* entire figure visible */
  border: none;
}

.swiper-pagination {
  margin-top: 1rem;
}

/* Responsive */
@media (max-width: 700px) {
  .swiper-slide img { width: 86vw; height: auto; }
  .figure-frame { height: 50vw; }
  .carousel-wrapper { padding: 0 1rem; }
}
</style>

<!-- ====== Init scripts ====== -->
<script>
document.addEventListener('DOMContentLoaded', function () {
  if (typeof Swiper === 'undefined') return;

  // IMAGES SLIDER (fancy coverflow)
  new Swiper('.imagesSwiper', {
    effect: 'coverflow',
    grabCursor: true,
    centeredSlides: true,
    slidesPerView: 'auto',
    loop: false,
    spaceBetween: 16,
    coverflowEffect: { rotate: 18, stretch: 0, depth: 120, modifier: 1, slideShadows: true },
    pagination: { el: '.imagesSwiper .swiper-pagination', clickable: true }
  });

  // FIGURES SLIDER (full figure visible, no zoom)
  new Swiper('.figuresSwiper', {
    slidesPerView: 1,           // only 1 figure visible at a time
    spaceBetween: 16,
    loop: false,
    pagination: { el: '.figuresSwiper .swiper-pagination', clickable: true }
  });
});
</script>

<style>
  .question-box {
    background: #0a4fffde;
    background: var(--qbox-bg, #0a4fffde);
    color: white;                          
    padding: 1.2rem 1.6rem;
    border-radius: 12px;
    margin: 1.8rem 0;
    border: 2px solid rgba(255, 255, 255, 0.1);
    box-shadow: 0 6px 18px rgba(0,0,0,0.18);
  }

  .question-box-title {
    font-weight: 800;
    font-size: 1.15rem;
    text-transform: uppercase;
    margin-bottom: 0.6rem;
    letter-spacing: 0.06em;
  }

  html[data-theme="dark"] .question-box {
    --qbox-bg: #003cbd;
    border-color: rgba(255,255,255,0.15);
    box-shadow: 0 8px 24px rgba(0,0,0,0.5);
  }
</style>

<div class="question-box">
  <div class="question-box-title">Key Questions</div>
  <ul>
    <li>Did posting BR videos accelerate channel growth ?</li>
    <li>Did existing creators pivot to BR content ?</li>
    <li>Were BR-focused creators more "opportunistic" ?</li>
    <li>Did creators abuse BR tags for visibility ?</li>
    <li>Did BR introduce new video formats (length, frequency) ?</li>
    <li>Did BR introduce new video formats (length, frequency) ?</li>
  </ul>
</div>

test test

