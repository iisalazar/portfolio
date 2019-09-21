<template>
  <div>
    <LandingBanner @clicked="CLICKED()"/>
    <SkillsSection/>
    <FeaturedProjects />
    <Footer />
  </div>
</template>

<script>
import LandingBanner      from '@/components/LandingBanner.vue'
import SkillsSection      from "@/components/Skills.vue"
import FeaturedProjects   from "@/components/FeaturedProjects.vue"




export default {
  name: 'home',
  components: {
    LandingBanner,
    SkillsSection,
    FeaturedProjects,
  },
  methods: {
  	CLICKED() {
  		console.log("kjaskldjlk")
  	}
  }
}
</script>
