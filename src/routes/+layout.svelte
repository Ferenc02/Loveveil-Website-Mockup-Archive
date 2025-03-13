<script>
	import Header from '../Header.svelte';
	import '../app.css';
	import '../index.css';
	import Footer from './Footer.svelte';
</script>

<body>
	<Header />

	<main>
		<slot />
	</main>
	<Footer />
</body>

<style lang="scss">
	body {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		width: 100%;
		box-sizing: border-box;
		padding: 1rem;
	}
</style>
