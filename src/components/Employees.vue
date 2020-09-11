<template>
  <div class="employee" >
    <div class="content">
      <vueper-slides
        class="no-shadow"
        :visible-slides="3"
        :gap="3"
        :autoplay="true"
        :slide-ratio="0.3"
        :duration="4000"
        :pauseOnHover="true"
        :dragging-distance="200"
        slide-content-outside="bottom"
        
      >
        
        <vueper-slide 
          class="shadow"
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
        title: 'Peder Gunnersen',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1681010/pexels-photo-1681010.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Pudder Gendersen',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/220453/pexels-photo-220453.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Gender Pudersen',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/774909/pexels-photo-774909.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
      },
      {
        title: 'Glemme Bindersen',
        content: 'Slide content.',
        image: "https://images.pexels.com/photos/1239291/pexels-photo-1239291.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260"
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