<template>
  <div>
    <carousel 
    :per-page="1" 
    :mouse-drag="true"
    :autoplay="true"
    :speed="600">
      <slide class="carousel carousel-inner">
        <div class="row">
        <div class="">
          <img :src="slideOneImage" alt="">
        </div>
        </div>
        
      </slide>
      <slide  class="carousel carousel-inner">
        <div class="row">
        <div class="">
          <img :src="slideTwoImage" alt="">
        </div>
        </div>
        
      </slide>
  </carousel>
  </div>
</template>

<script>

import { Carousel, Slide } from 'vue-carousel';

 export default {
   name: 'Slider',
   data() {
     return {
       slideOneImage: 'https://i.picsum.photos/id/1002/4312/2868.jpg?hmac=5LlLE-NY9oMnmIQp7ms6IfdvSUQOzP_O3DPMWmyNxwo',
       slideTwoImage: 'https://i.picsum.photos/id/1032/2880/1800.jpg?hmac=5SLBdyPZBMyr5IBkIRfffZV10bP87Y7RrxVZX1vCefA',
     }
   },
   components: {
    Carousel,
    Slide
  }
  }
</script>

<style lang="scss">
  div {
    .VueCarousel {
      max-height: 100vh;
      position: relative;
    
      .VueCarousel-pagination {
        width: 100%;
        text-align: center;
        position: absolute;
        bottom: 0;

        .VueCarousel-dot-container {
          margin: 0;

          button.VueCarousel-dot {
            width: 50px!important;
            height: 4px!important;
            border-radius: 0;
            outline: none;
          }
        }
      }
    }
  
  
  }
</style>