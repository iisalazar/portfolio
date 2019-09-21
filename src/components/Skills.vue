<template>
	<section class="section">
		<div class="container">
			<div class="columns is-desktop is-8">
				<div class="column">
					<div class="title header">
						Skills
					</div>
					<div class="subtitle caption">
						This are my skills
					</div>	
					<ul>
						<li 
							v-for="skill, index in skills"
							:key="index"
							>
							{{ skill }}
						</li>
					</ul>
				</div>
				<div class="column">
					<div class="level">
						<figure class="level-item image is-64x64"
							v-for="icon, index in icons"
							:key="index"
							>
							<img 
								:src="getImgUrl(icon)" />
						</figure>
						
					</div>
				</div>
			</div>
		</div>
	</section>
</template>
<script>
export default {
	name: "SkillsSection",
	data() {
		return {
			skills: [
				"Front end development using vue js",
				"Back end development using flask / django / express"
			],
			icons: [
				'flask',
				'python',
				'django',
				'vuejs'
			]
		}
	},
	methods: {
		getImgUrl(img){
			return require('@/assets/img/' + img + '.png')
		}
	}
}
</script>
<style type="text/css" scoped>
.section {
	height: 325px;
	padding: 5em 1em;
}
.icon {
	height: 50px;
	width: 50px;
}
figure {
	padding: 1em;
	margin: 10% 0 10% 0;
}
</style>