<template>
  <nav class="nav">
  	<div class="logo">
			<a href="#" class="logo">
				<h2>
					MyPlants.app
				</h2>
			</a>
  	</div>

		<span class="subheader">Keep your plants alive</span>

  </nav>
</template>

<script>
export default {

}
</script>

<style>

nav {
	display: flex;
	justify-content: space-between;
	align-items: center;
	font-weight: lighter;
}

.nav .logo {
	display: flex;
	flex-direction: column;
	justify-content: center;
}

.nav .logo .subheader {
	opacity: .070;
	font-size: 1rem;
	color: white;
}

.nav .nav-content {
	font-size: 1rem;
}

.nav-content ul {
	display: flex;
	list-style: none;
}

.nav-content ul li {
	padding: 2px 10px;
}

.nav-content ul li:not(:first-of-type) {
	border-left: 1px solid rgba(255, 255, 255, .5)
}

</style>
