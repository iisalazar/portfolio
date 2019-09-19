<template>
  <div class="banner">
    <div class="bg">
      <div class="columns content is-desktop">
        <div class="column">
          HELLO
        </div>
        <div class="column">
          HELLO
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "LandingBanner"
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
}

.banner .bg {
  background-color: rgba(0, 0, 0, 0.6);
  width: 100%;
  height: 100%;
}
</style>
