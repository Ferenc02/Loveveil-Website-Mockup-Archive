<script>
	import undraw from '$lib/images/undraw4.svg';
	import klippan from '$lib/images/klippan_swe.webp';
	import Donate from '../Donate.svelte';
</script>

<svelte:head>
	<title>About LoveVeil: Our Story of Authentic Connections</title>
	<meta
		name="description"
		content="Discover the story behind LoveVeil: where the idea for authentic connections bloomed into reality. Join us on our journey to reshape online dating."
	/>
</svelte:head>
<hgroup>
	<article>
		<h1>Our Journey: From Idea to Reality At LoveVeil</h1>
		<div class="text_container split">
			<div>
				<p>
					We're on a mission to redefine online dating and foster authentic connections. Our journey
					began right here in Sweden, Gothenburg, a country known for its beautiful landscapes,
					innovation, and a strong sense of community.
				</p>

				<p>
					The idea for LoveVeil was born out of a simple yet profound realization: in the digital
					age, we've lost some of the magic of getting to know someone. Swiping through photos and
					superficial profiles left us yearning for something more genuine.
				</p>
				<p>
					We envisioned a dating app where meaningful conversations take precedence over
					appearances. Drawing inspiration from the rich culture of Sweden, where open communication
					and authenticity are highly valued, we embarked on a journey to create a platform that
					reflects these principles.
				</p>
				<p>
					We believe that connections based on shared interests, values, and deep conversations are
					the ones that stand the test of time.
				</p>
			</div>
			<img src={undraw} alt="open illustration of a team" class="image_inherit undraw mini_hover" />
		</div>
	</article>

	<article>
		<h2>Founder's Story</h2>
		<div class="founder_container">
			<p>
				At the heart of LoveVeil stands a visionary founder, a dynamic individual with roots in both
				Sweden and Hungary. A self-learned engineer and years of experience in programming and web
				development, but also a dreamer with a unique vision - to revolutionize the dating
				landscape.
			</p>
			<p>
				The journey into the world of dating apps began with a simple yet profound observation. In a
				world dominated by superficiality, the founder envisioned an alternative, where meaningful
				connections would take precedence over appearances. It was this vision that fueled the
				creation of LoveVeil.
			</p>
			<p>
				LoveVeil has the potential to transform how people form connections in the digital age. It's
				an exciting vision, one that we invite you to be a part of.
			</p>
		</div>
		<div class="klippan_container">
			<img
				src={klippan}
				alt="Landscape view of Sweden Gothenburg Klippan"
				class="image_inherit mini_hover klippan"
			/>
			<p class="disclaimer">Landscape view of Sweden Gothenburg Klippan</p>
		</div>
		<p>
			But to truly bring this vision to life, we need your support. LoveVeil is not just a dating
			app; it's a mission to redefine how we connect in an increasingly digital world. Your generous
			contributions can help us develop innovative features, ensure the highest level of security
			and privacy, and expand our reach to help more people find meaningful connections. <br /><br
			/>Together, we can make this dream a reality. Join us in this exciting journey by becoming a
			donor and playing a vital role in reshaping the future of online dating. Every donation brings
			us one step closer to our vision of authentic, meaningful connections for all.
		</p>
	</article>
	<article class="donate_container">
		<Donate />
	</article>
</hgroup>

<style lang="scss">
	h1 {
		padding-bottom: 1.5rem;
	}
	h2 {
		padding: 1rem;
		font-weight: 600;
		color: var(--primary-color-darker);
		text-align: center;
	}
	p {
		font-weight: 300;
		font-size: 1.2rem;
		padding: 1rem;
	}
	article {
		padding-bottom: 2rem;
	}

	.split {
		display: flex;
		flex-flow: row wrap;
		div {
			@media screen and (min-width: 1858px) {
				width: 50%;
			}

			p {
				padding: 1rem;
			}
		}
		justify-content: center;
	}
	.undraw {
		@media screen and (max-width: 1300px) {
			height: 100%;
			width: 100%;
			margin: 2rem 0;
		}
	}
	.donate_container {
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 0.5rem;
	}
	.klippan_container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		.klippan {
			max-width: 60rem;
			@media screen and (max-width: 1300px) {
				height: 100%;
				width: 100%;
				margin: 0.5rem 0;
			}
		}
		p {
			font-size: smaller;
			padding: 0.5rem 1rem;
			color: var(--text-primary-lighter);
		}

		padding: 2rem 0;
		@media screen and (max-width: 1300px) {
			padding: 0;
		}
	}
</style>
