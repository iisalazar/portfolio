<template>
  <div>
    <LandingBanner @clicked="CLICKED()"/>
    <SkillsSection/>
  </div>
</template>

<script>
import LandingBanner from '@/components/LandingBanner.vue'
import SkillsSection from "@/components/Skills.vue"

export default {
  name: 'home',
  components: {
    LandingBanner,
    SkillsSection
  },
  methods: {
  	CLICKED() {
  		console.log("kjaskldjlk")
  	}
  }
}
</script>
