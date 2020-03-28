<template>
  <section class="container">
    <b-navbar>
      <template slot="start">
        <b-navbar-item href="#">
          Projects
        </b-navbar-item>
        <b-navbar-item href="#">
          About
        </b-navbar-item>
        <b-navbar-item href="#">
          Contact
        </b-navbar-item>
      </template>
    </b-navbar>
    <header class="section columns">
      <div class="column is-half">
        <h1>
          Víctor Villalobos is a
          <vue-typed-js
            :type-speed="100"
            :start-delay="100"
            :back-delay="100"
            :back-speed="100"
            :loop="true"
            :strings="['Backend Developer.', 'Frontend Developer.', 'DevOps.']"
          >
            <span class="typing" />
          </vue-typed-js>
        </h1>
      </div>
      <div class="column header-image is-half">
        <img
          src="~/assets/img/header.png"
          srcset="~/assets/img/header2x.png 2x"
          alt="people-working"
        >
      </div>
    </header>
    <main class="content">
      <nuxt />
    </main>
  </section>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style lang="scss">

@import '~/static/scss/pages/home.scss';

</style>
