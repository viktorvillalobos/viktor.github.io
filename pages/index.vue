<template>
  <section class="projects">
    <h2>Projects</h2>
    <div class="projects-wrapper columns is-desktop is-multiline">
      <project class="column" />
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
    }
  }
}
</script>
