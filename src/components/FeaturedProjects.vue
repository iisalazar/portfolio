<template>
	<div class="container">
		<div class="tile is-ancestor">
			<div class="tile is-vertical is-4 is-vertical is-parent">
				<div class="tile is-child box">
					<p class="title header">Projects</p>
	        		<p class="subtitle caption">A list of my featured projects</p>
				</div>
				<div class="tile is-child box">
	        		<p class="subtitle caption">For a list of all my projects, you can visit <a href="#">here</a></p>
				</div>
			</div>
			 <div class="tile is-parent is-8">
				  <article class="tile is-child box">
				    <div class="content">
				    	<div class="columns is-desktop">
				    		<div v-for="project, index in projects" class="column">
				    			<div class="card">
				    				<div class="card-header">
				    					<p class="card-header-title">
				    						{{ project.title }}
				    					</p>
				    				</div>
						          	<div class="card-content">
						          		<div class="content">
						          			{{ project.description }}
						          		</div>
						          	</div>
						        </div>	
				    		</div>
				    	</div>
				    </div>
				  </article>
				</div>
		  </div>
		</div>		
</template>
<script>
	
export default {
	name: "FeaturedProjects",
	data() {
		return {
			projects: [
				{
					title: "Test project",
					description: "Test project"
				},
				{
					title: "Test project",
					description: "Test project"
				},
				{
					title: "Test project",
					description: "Test project"
				},
				{
					title: "Test project",
					description: "Test project"
				}
			]
		}
	}
}
</script>
<style scoped>
.container {
	padding: 1em;
}
</style>