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
          description: `Talana is a Payroll & and Asistence platform focused in make people happy by
                     helping to automate the internal processes of companies and communication with their
                     employees process using innovative software solutions,i currently 
                     work as a Backend Developer & DevOps, mainly implementing microservices, and 
                     helping to improve the k8s infrastructure and monitoring services.`,
          url: 'https://talana.com/',
          images: [
            { webp: '/projects/talana/talana-employee-record-black.webp', img: '/projects/talana/talana-employee-record-black.png', color: 'primary' },
            { webp: '/projects/talana/talana-employee-record-black.webp', img: '/projects/talana/talana-dashboard-record-black.png', color: 'primary' }
          ]
        },
        {
          title: 'Adslab',
          subtitle: 'Teach Lead & Founder',
          description: `Adslab is a startup that tries to innovate in marketing online, allowing to
                        publish ads in free ads sites, also handle multiple client projects.`,
          url: 'https://adslab.io/',
          images: [
            { webp: '/projects/adslab/adslab-landing-1.webp', img: '/projects/adslab/adslab-landing-1.png', color: 'primary' },
            { webp: '/projects/adslab/adslab-landing-2.webp', img: '/projects/adslab/adslab-landing-2.png', color: 'primary' },
            { webp: '/projects/adslab/adslab-landing-3.webp', img: '/projects/adslab/adslab-landing-3.png', color: 'primary' },
            { webp: '/projects/adslab/adslab-landing-4.webp', img: '/projects/adslab/adslab-landing-4.png', color: 'primary' },
            { webp: '/projects/adslab/adslab-landing-5.webp', img: '/projects/adslab/adslab-landing-5.png', color: 'primary' },
            { webp: '/projects/adslab/adslab-landing-6.webp', img: '/projects/adslab/adslab-landing-6.png', color: 'primary' }
          ]
        },
        {
          title: 'Pythonist.dev',
          subtitle: 'Writer & Founder',
          description: 'Spanish articles about python development.',
          url: 'https://pythonist.dev/',
          images: [
            { webp: '/projects/pythonist/pythonist-dev-1.webp', img: '/projects/pythonist/pythonist-dev-1.png', color: 'primary' },
            { webp: '/projects/pythonist/pythonist-dev-2.webp', img: '/projects/pythonist/pythonist-dev-2.png', color: 'primary' },
            { webp: '/projects/pythonist/pythonist-dev-3.webp', img: '/projects/pythonist/pythonist-dev-3.png', color: 'primary' }
          ]
        }
      ]
    }
  }
}
</script>
