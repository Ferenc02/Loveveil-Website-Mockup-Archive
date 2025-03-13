<script>
	import patreon_logo from '$lib/images/patreon_logo.png';
</script>

<div class="donation_buttons_container">
	<a href="#" target="_blank" class="patreon_button mini_hover"
		><img src={patreon_logo} alt="Patreon Logo" />Support Us On Patreon</a
	>
</div>

<style lang="scss">
	.donation_buttons_container {
		display: flex;
		flex-flow: row wrap;
		justify-content: center;
		gap: 0.5rem;

		@media screen and (min-width: 1000px) {
			justify-content: flex-start;
		}
		a {
			padding: 0.33rem 1rem 0.33rem 0.5rem;
			margin-top: 0.75rem;
			border-radius: 0.75rem;
			text-transform: uppercase;
			font-weight: 500;
			font-size: 1.05rem;
			display: flex;
			justify-content: center;
			align-items: center;
			width: fit-content;
			color: var(--text-primary-inverse);

			/*Mobile*/
			@media screen and (max-width: 1000px) {
			}
		}
		img {
			width: 3rem;
			margin-right: 0.5rem;
		}
		/*Patreon Button*/
		.patreon_button {
			background-color: var(--patreon-background);
		}
		.kickstarter_button {
			background-color: var(--indiegogo-background);
		}
	}
</style>
