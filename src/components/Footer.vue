<template>
	<footer class="footer">
	  <div class="content has-text-centered">
	    <div class="text">
	      Stay connected
	    </div>
	    <img 
	    	v-for="img, index in social_media" 
	    	:src="getImgUrl(img.name)" 
	    	@click="goTo(img.url)"
	    	width="40"
	    	/>
	  </div>
	</footer>
</template>
<script>
export default {
	name: "Footer",
	data() {
		return {
			social_media: [
				{
					name: 'twitter',
					url: 'https://twitter.com/theiansalazar'
				},
				{
					name: 'github',
					url: 'https://github.com/dertrockx'
				},
				{
					name: 'instagram',
					url: 'https://www.instagram.com/dertrockx/'
				}
				]
		}
	},
	methods: {
		getImgUrl(img){
			return require('@/assets/img/' + img + '.png')
		},
		goTo(url){
			console.log(url)
			window.open(url);
		}
	}
}
</script>
<style scoped>

footer {
	padding: 3em;
	background: #363636;
}

footer * {
	color: white;
}
img {
	margin: 0 0.5em;
}
</style>