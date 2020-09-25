<template>
  <div class="employee py-5" >
    <div class="content">
      <vueper-slides
        class="no-shadow"
        :breakpoints='breakpointsSlides'
        :visible-slides="3"
        :gap="3"
        :autoplay="true"
        :slide-ratio="0.3"
        :duration="6000"
        :pauseOnHover="true"
        :dragging-distance="100"
        slide-content-outside="bottom"
        ref="vueperSlides"
      >
        <vueper-slide 
          :breakpoints='breakpointsSlide'
          class="shadow"
          v-for="(slide, idx) in slides" 
          :key="slide.title" 
          :title="slide.title"
          :image="slide.image"
          @click.native="setSlide(idx)"
        > 
        <template v-slot:content>
          <div class="employee-name mx-auto col text-center">
            <h3>{{ slide.title }}</h3>
            <p>{{slide.content}}</p>
          </div>
        </template>
        </vueper-slide>
      </vueper-slides>
    </div>
  </div>
</template>

<script>

import { VueperSlides, VueperSlide } from 'vueperslides'

export default {
  components: {VueperSlides, VueperSlide},
  props: {},
  data: () =>  ({
    slides: [
      {
        title: 'Gunner Pedersen',
        content: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Peder Gunnersen',
        content: 'Loremtry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also',
        image: "https://images.pexels.com/photos/1681010/pexels-photo-1681010.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Pudder Gendersen',
        content: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also',
        image: "https://images.pexels.com/photos/220453/pexels-photo-220453.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Gender Pudersen',
        content: 'Lorem Ipsum is simply dummy text of the printing aaklshdsklahdkjsahdkshakjdas',
        image: "https://images.pexels.com/photos/774909/pexels-photo-774909.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Glemme Bindersen',
        content: 'Lo Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only fivbook. It has survived not only book. It has survived not only e centurdsadsadasdies, but also',
        image: "https://images.pexels.com/photos/1239291/pexels-photo-1239291.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      }
    ],
    breakpointsSlides: {
      992: {
        visibleSlides: 2,
        slideRatio: 0.5,
        
      },
      768: {
        visibleSlides: 1,
        slideRatio: 1,
      },
    },
  }),
  computed: {
  },
  methods: {
    setSlide(idx) {
      this.$refs.vueperSlides.goToSlide(idx)
    }
  },
  mounted() {
  }
}
</script>

<style lang="scss">

  .employee {
    background-color: #f4f8f7;
  }

  .vueperslide {
    transform: scale(0.7);
    transition: all 0.3s;
    cursor: pointer;
    border-radius: 50%;
  }

  .vueperslide--active {
    transform: scale(0.9);
  }

  .vueperslides__bullet--active .default {
    border-color: #30c9e8!important;
  }

  .vueperslides__arrow {
    color: #3c4a4d;
  }

  .employee-name {

    flex-direction: row; 
    white-space:pre-line; 
    width: 70%;

    & p {
      font-size: 20px;
    }
  }

  @media only screen and (max-width: 992px) {

    .employee .content {
      width: 70%;
    }

    .employee-name {
      width: 80%;
    }

  }
  @media only screen and (max-width: 768px) {

    .employee .content {
      width: 70%;
    }

    .vueperslide {
      transform: scale(1);
    }

    .vueperslide--active {
      transform: scale(1);
      box-shadow: 0 0 0 rgba(0,0,0,.15)!important;
    }

    .employee-name {
      width: 100%;
      margin-top: 15px;
    }

  }

</style>