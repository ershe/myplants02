<template>
	<div class="bigbox">
		<div class="grid">
			<div class="card-style sidebar">
			</div>
			<div class="card-style card-logo">
				<img class="img-cover" src="https://www.dmu.edu/wp-content/uploads/2019/08/poison-ivy_splash-plain.jpg">
			</div>
			<div id="shifter" class="card-style card-title flexbox">
			  <h1>{{ post.title }}</h1>
			</div>
			<div class="card-style card-subtitle">
				<div class="">
					<h2>This site is a test for creating a personal plant database and to potentially scale this.</h2>
				</div>
			</div>
			<div class="card-style card-body">
				<div>
					<p>Why do this? To learn Javascript, Vue.js, Nuxt.js, APIs, and generally the JAMStack.</p>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data () {
		return {
			id: this.$route.params.id,
			posts: [
				{
					id: 'myplants',
					title: 'My Houseplants Are Happy',
					content: 'This site is a test for creating a personal plant database and to potentially scale this',
				},
				{
					id: 'whyHouseplants',
					title: 'Why Houseplants?',
					content: 'Why do this? To learn Javascript, Vue.js, Nuxt.js, APIs, and generally the JAMStack.',
				},
				{
					id: 'howPlants',
					title: 'How to care for your plants!',
					content: 'Step 1, Step 2, Step 3, easy peasy abcd',
				},
			]
		}
	},
	computed: {
		post () {
			return this.posts.find(post => post.id === this.id)
		}
	}
}
</script>

<style>
</style>
