<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation, Pagination, Autoplay } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
</script>

<template>
  <div class="spacing"></div>
  <div class="clothes">
    <h3>Vestuário</h3>
    <swiper
        :modules="[Navigation, Pagination, Autoplay]"
        :spaceBetween="10"
        :slidesPerView="1"
        :navigation="true"
        :pagination="{ clickable: true }"
        :autoplay="{ delay: 3000, disableOnInteraction: false }"
        class="swiper-container"
    >
      <swiper-slide>
        <img src="@/assets/vestuario-1.png" alt="Vestuário 1" />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/vestuario-2.png" alt="Vestuário 2" />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/about-me-photo.png" alt="Vestuário 3" />
      </swiper-slide>
    </swiper>
  </div>
</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

.clothes {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h3 {
  font-family: 'Raleway', sans-serif;
  font-size: 6vw;
  font-weight: lighter;
  margin-bottom: 2rem;
}

.swiper-container {
  width: 100%;
  max-width: 600px;
  height: auto;
}

img {
  width: 100%;
  max-width: 500px;
  height: auto;
  display: block;
  margin: 0 auto;
}

@media (max-width: 1024px) {
  h3 {
    font-size: 5vw;
  }
}

@media (max-width: 768px) {
  h3 {
    font-size: 5.5vw;
  }
}
</style>
