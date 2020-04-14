<template>
  <div class="project-item column is-10 is-offset-1">
    <div class="project-header columns is-desktop">
      <div class="project-description column is-8 is-offset-1">
        <p class="project-title title is-size-3">
          {{ title }}
        </p>
        <p class="project-subtitle is-size-5">
          {{ subtitle }}
        </p>
        <p class="project-description">
          {{ description }}
        </p>
      </div>
      <div class="show-work column is-2">
        <b-button type="is-danger" size="is-medium" tag="a" target="_blank" :href="url">
          Show work
        </b-button>
      </div>
    </div>
    <div class="project-content">
      <b-carousel class="column is-10 is-offset-1" :indicator-inside="false" :overlay="gallery">
        <b-carousel-item v-for="(item, i) in images" :key="i">
          <picture>
            <source v-lazy-load :srcset="item.webp" alt="img" type="image/webp">
            <img v-lazy-load :src="item.img" alt="img">
          </picture>
        </b-carousel-item>
      </b-carousel>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Project',
  props: {
    title: {
      type: String,
      required: true
    },
    subtitle: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    url: {
      type: String,
      required: true
    },
    images: {
      type: Array,
      required: true
    }
  },
  data () {
    return {
      gallery: false
    }
  }
}
</script>
