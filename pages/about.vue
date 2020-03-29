<template>
  <section class="aboutme">
    <h2>About</h2>
    <div class="about-wrapper columns is-desktop">
      <div class="column is-3 networks">
        <p class="title">
          Let's Connect
        </p>
        <div class="socials">
          <a href="https://www.linkedin.com/in/viktor-villalobos/">LinkedIn ></a>
          <a href="https://www.instagram.com/viktordeveloper/">Instagram ></a>
          <a href="https://github.com/viktorvillalobos">Github ></a>
          <a href="https//freelancer.com/u/revxfire">Freelancer ></a>
          <a href="https://www.indiehackers.com/ViktorDeveloper">Indie Hackers ></a>
          <a href="https://stackoverflow.com/users/2202/victor-villalobos">StackOverFlow ></a>
          <a href="https://es.stackoverflow.com/users/2202/victor-villalobos">StackOverFlow Spanish ></a>
        </div>
        <div class="photo">
          <img src="~/assets/img/profile.jpeg" alt="profile photo">
        </div>
      </div>
      <div class="column is-8 is-offset-1 about">
        <p class="subtitle is-size-4 has-text-weight-bold">
          Hello Hola Hallo!
        </p>
        <p>
          I'm Víctor Villalobos, a hands on software developer &amp; DevOps
          who works collaboratively with other engineers, executives and
          business partners to create consumer and enterprise, integrated
          hardware and software product experiences. Currently, I am a
          Full Stack Developer &amp; DevOps in <a href="https://talana.com/">Talana</a>.
        </p>

        <p>
          Most recently, i worked in  <a href="https://adslab.io">Adslab</a> an advertising saas platform who use scraping to make easy publish ads in mutiple free ads sites,
          using scrapers to put ads in sites and generatic metrics for the user.
        </p>
        <p>
          Prior to Adslab, i worked as Tech Leader and Founder in Firesoft.org, a digital agency, who deliver more than 100 products in two years for more than 60 customers
          around the world, during this time we create E-Commerse, SaaS platforms and many others interesting projects.
        </p>
        <p>
          Over the last year i am studying Data Science and Machine learning, to complement my knowledge as Sofware Developer.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HomePage',
  components: {},
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

<style lang="scss">
  @import '~/assets/scss/pages/about.scss'
</style>
