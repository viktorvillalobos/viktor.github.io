<template>
  <section class="projects">
    <h2>Projects</h2>
    <div class="projects-wrapper columns is-desktop is-multiline">
      <project
        v-for="(project, idx) in projects"
        :key="idx"
        class="column"
        :title="project.title"
        :subtitle="project.subtitle"
        :description="project.description"
        :images="project.images"
        :url="project.url"
      />
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
      projects: [
        {
          title: 'Talana',
          subtitle: 'Backend rest services and microservices',
          description: `Talana is a Payroll & and Asistence platfor focused in make people happy, 
                     helping in automate companies process using innovative software,i currently 
                     work as Backend Developer & DevOps, implementing microservices, and 
                     helping to improve the infrastructure.`,
          url: 'https://talana.com/',
          images: [
            { img: '/projects/talana/talana-employee-record-black.png', color: 'primary' },
            { img: '/projects/talana/talana-dashboard-record-black.png', color: 'primary' }
          ]
        },
        {
          title: 'Adslab',
          subtitle: 'Teach Lead & Founder',
          description: `Adslab is a startup that tries to innovate in marketing online, allowing to
                        publish ads in free ads sites, also handle multiple client projects.`,
          url: 'https://adslab.io/',
          images: [
            { img: '/projects/adslab/adslab-landing-1.png', color: 'primary' },
            { img: '/projects/adslab/adslab-landing-2.png', color: 'primary' },
            { img: '/projects/adslab/adslab-landing-3.png', color: 'primary' },
            { img: '/projects/adslab/adslab-landing-4.png', color: 'primary' },
            { img: '/projects/adslab/adslab-landing-5.png', color: 'primary' },
            { img: '/projects/adslab/adslab-landing-6.png', color: 'primary' }
          ]
        }
      ]
    }
  }
}
</script>
