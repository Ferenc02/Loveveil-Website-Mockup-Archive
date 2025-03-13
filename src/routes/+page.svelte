<script>
	import locked_app_image from '$lib/images/locked_app.png';
	import unlocked_app_image from '$lib/images/unlocked_app.png';
	import Donate from './Donate.svelte';
</script>

<svelte:head>
	<title>Unlock Meaningful Connections: Explore LoveVeil - Your Path to Deeper Bonds</title>
	<meta
		name="description"
		content="Discover LoveVeil: Where conversations unveil connections. Join now for authentic conversations and meaningful relationships. Unblur your love story today."
	/>
	<meta property="og:image" content={unlocked_app_image} />
</svelte:head>

<section>
	<div class="presentation_container">
		<div class="title_container">
			<h1 class=" ">
				Love Beyond the Surface <span class="poetsenOne">LoveVeil</span>
				Where Blur Blossoms into True Connection!
			</h1>
			<p>
				Unlock meaningful connections for free – no subscription fees, just authentic connections.
			</p>
			<Donate />
			<a href="/app" class="learn_more medium_hover"
				><span>Learn More</span> <span class="material-symbols-outlined"> chevron_right </span></a
			>
		</div>
		<div class="images_container image_inherit">
			<div class="image_container image_inherit">
				<img src={locked_app_image} alt="Locked section mockup of the app" class="image_inherit" />
				<img
					src={unlocked_app_image}
					alt="Unlocked section mockup of the app"
					class="image_inherit"
				/>
			</div>
		</div>
	</div>
</section>

<style lang="scss">
	section {
		display: flex;
		flex-direction: column;
		justify-content: space-between;

		.presentation_container {
			display: flex;
			justify-content: center;
			align-items: center;
			max-height: fit-content;
			padding: 0.5rem;
			flex-flow: row wrap;

			@media screen and (min-width: 1000px) {
				padding: 2rem;
			}
			.title_container {
				@media screen and (min-width: 1000px) {
					margin: 4rem;
					width: 50%;
				}
				p {
					font-size: 1.1rem;
					font-weight: 300;
					padding: 0.5rem 0rem;
				}
				h1 {
					font-size: 2rem;
					@media screen and (min-width: 1000px) {
						font-size: 3rem;
						line-height: 1.375;
					}
				}
			}
			.images_container {
				display: flex;
				flex-direction: column;
				align-items: center;
				.image_container {
					display: flex;
					flex-flow: row wrap;
					justify-content: center;
					img {
						max-height: 40rem;
					}
				}
			}
		}
	}

	.learn_more {
		color: var(--link-primary-color);
		display: flex;
		padding: 1.25rem 0.5rem;
		font-size: larger;
		justify-content: center;
		width: 100%;
		height: 100%;

		align-items: center;

		/*desktop*/
		@media screen and (min-width: 1000px) {
			width: fit-content;
		}
	}

	@media screen and (max-width: 480px) {
	}
</style>
