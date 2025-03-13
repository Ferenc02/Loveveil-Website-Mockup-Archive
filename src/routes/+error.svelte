<script>
	import errorImage from '$lib/images/undraw_error.svg';
</script>

<svelte:head>
	<title>LoveVeil - Page Not Found</title>
	<meta
		name="description"
		content="Oops! It looks like you've ventured into uncharted territory on LoveVeil. Don't worry; we'll help you find your way back to meaningful connections"
	/>
</svelte:head>
<div class="img_container">
	<img src={errorImage} alt="error 404" />
</div>

<style lang="scss">
	.img_container {
		display: flex;
		justify-content: center;
		padding: 2rem;
	}
	img {
		max-width: 20rem;
		@media screen and (min-width: 1000px) {
			max-width: 40rem;
		}
	}
</style>
