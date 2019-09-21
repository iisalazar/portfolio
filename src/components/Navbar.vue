<template>
	<nav class="navbar is-fixed-top is-black" role="navigation" aria-label="main navigation">
		<div class="container">
			<div class="navbar-brand">
				<a class="navbar-item text" href="https://bulma.io">
					Ian Salazar
				</a>

				<a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" @click="active = !active">
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
				</a>
			</div>

			<div id="navbarBasicExample" 
				class="navbar-menu" 
				:class="{ 'is-active': active }"
				>
				<div class="navbar-start">
					<a class="navbar-item caption" href="#">
						Projects
					</a>
				</div>
				<div class="navbar-end">
					<a class="navbar-item caption" href="#">
						Contact
					</a>
				</div>			
			</div>
		</div>
	</nav>
</template>
<script>
export default {
	name: "Header",
	data() {
		return {
			active: false
		}
	}
}
</script>