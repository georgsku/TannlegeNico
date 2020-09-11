<template>
  <div class="employee" >
    <div class="content">
      <vueper-slides
        class="no-shadow"
        :visible-slides="3"
        :gap="3"
        :autoplay="true"
        :slide-ratio="0.3"
        :duration="2000"
        :pauseOnHover="true"
        :dragging-distance="200"
        slide-content-outside="bottom"
        
      >
        
        <vueper-slide 
          v-for="slide in slides" 
          :key="slide.title" 
          :title="slide.title"
          :image="slide.image"
        > 
        <template v-slot:content>
          <div class="vueperslide__content-wrapper employee-name" style="flex-direction: row">
            <p>{{ slide.title }}</p>
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
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Slide #2',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Slide #3',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Slide #4',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Slide #5',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1933873/pexels-photo-1933873.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      }
    ]
  }),
  computed: {
  },
  methods: {
  },
  mounted() {
  }
}
</script>

<style lang="scss">

  .employee {
    margin: 30px auto;
  }

  .vueperslide {
    transform: scale(0.8);
    transition: all 0.3s;
  }

  .vueperslide--active {
    transform: scale(1);
  }

  .employee-name {

    & p {
      font-size: 20px;
    }
  }

</style>