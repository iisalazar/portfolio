<template>
  <div class="banner">
    <div class="bg">
      <div class="columns content is-desktop">
        <div class="column">
          <div class="header">
            Ian Salazar
          </div>
          <div class="caption">
            Self-taught back-end and front-end developer and hackathon participant.
          </div>
        </div>
        <div class="column">
          <b-button 
            rounded 
            inverted 
            outlined 
            type="is-dark" 
            size="is-large"
            @click="clicked()"
            >
            Learn More
          </b-button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "LandingBanner",
    methods: {
      clicked() {
        console.log("Clicked from inside")
        this.$emit('clicked')
      }
    }
  }
</script>
<style scoped>
.banner {
  background: url("../assets/banner.jpg") no-repeat center;
  background-size: cover;
	background-position: 100%;
	height: 640px;
	width: 100%;
}

.banner .content {
  padding: 15%;
  color: white;
  text-align: center;
}

.banner .bg {
  background-color: rgba(0, 0, 0, 0.6);
  width: 100%;
  height: 100%;
}
button {
  margin: 1.5em;
}

</style>
