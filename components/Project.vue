<template>
  <div class="project-item column is-10 is-offset-1">
    <div class="project-header columns is-desktop has-text-centered">
      <div class="project-description column is-8 is-offset-1">
        <p class="project-title title">
          Talana: the most bigger payroll platform in Latam.
        </p>
        <p class="project-subtitle">
          Backend services and authentication for talana employee profile, this handle
          more than 1700 companies and more than 100,000 employee monthly.
        </p>
      </div>
      <div class="show-work column is-2">
        <b-button type="is-danger" size="is-medium" tag="a" target="_blank" href="https://talana.com">
          Show work
        </b-button>
      </div>
    </div>
    <div class="project-content">
      <b-carousel class="column is-10 is-offset-1">
        <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
          <section :class="`hero is-medium is-${carousel.color}`">
            <div class="hero-body has-text-centered">
              <h1 class="title">
                {{ carousel.text }}
              </h1>
            </div>
          </section>
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
    icon: {
      type: String,
      required: true
    }
  },
  data () {
    return {
      carousels: [
        { text: 'Slide 1', color: 'primary' },
        { text: 'Slide 2', color: 'info' },
        { text: 'Slide 3', color: 'success' },
        { text: 'Slide 4', color: 'warning' },
        { text: 'Slide 5', color: 'danger' }
      ]
    }
  }
}
</script>
