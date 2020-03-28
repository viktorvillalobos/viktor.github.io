<template>
  <section class="section projects">
    <h2>Projects</h2>
    <div class="projects-wrapper columns is-mobile">
      <project />
    </div>
  </section>
</template>

<script>
import Project from '~/components/Project.vue'
export default {
  name: 'HomePage',

  components: {
    Project
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
