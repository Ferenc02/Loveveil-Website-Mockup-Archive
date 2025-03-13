<script defer lang="ts">
	import undraw from '$lib/images/undraw4.svg';
	import klippan from '$lib/images/klippan_swe.webp';
	import Donate from '../Donate.svelte';

	let faq_containers;

	let getAllFaq = (number: any) => {
		faq_containers = document.querySelectorAll('.faq_container');

		console.log(faq_containers[number]);

		faq_containers[number].classList.toggle('faq_closed');
	};
</script>

<svelte:head>
	<title>LoveVeil FAQ: Your Questions, Our Answers</title>
	<meta
		name="description"
		content="Explore LoveVeil's comprehensive FAQ for answers to common queries about our unique dating concept. Discover how we prioritize meaningful connections."
	/>
</svelte:head>
<h1>FAQ</h1>
<div class="faq_parent_container">
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(0)}>
		<div class="faq_title"><p>What is LoveVeil, and how does it work?</p></div>
		<div class="faq_text">
			<p>
				LoveVeil is a dating concept that values meaningful connections. Profiles start with blurred
				images, encouraging authentic conversations. As you chat, images gradually become clearer,
				revealing the person behind the photo. It's a fresh take on dating, putting conversations
				first. Curious to learn more? <a href="/app">Read more here.</a>
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(1)}>
		<div class="faq_title"><p>Is LoveVeil currently available for download?</p></div>
		<div class="faq_text">
			<p>
				LoveVeil is in the development stage and not available for download yet. We're working
				diligently to bring this exciting concept to life. Stay tuned for updates on our progress.
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(2)}>
		<div class="faq_title"><p>How can I donate?</p></div>
		<div class="faq_text">
			<p>
				We greatly appreciate your willingness to support LoveVeil's vision for authentic
				connections. To make a donation, you can join our Patreon community. <br /><br />Patreon:
				LoveVeil has a Patreon page where you can become a patron and support our development. By
				becoming a patron, you'll gain access to exclusive updates, behind-the-scenes content, and
				the opportunity to be part of our growing community.
				<br /><br />Your donations play a crucial role in helping us bring LoveVeil to life and
				reshape the dating landscape. Your support is invaluable, and we're grateful for every
				contribution.
				<Donate />
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(3)}>
		<div class="faq_title"><p>What sets LoveVeil apart from other dating apps?</p></div>
		<div class="faq_text">
			<p>
				LoveVeil stands out by reimagining the dating experience. We emphasize conversations and
				connection-building, allowing users to uncover each other's personalities before seeing
				clear profile images. Focusing on building connections rather than appearances.
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(4)}>
		<div class="faq_title"><p>When can I expect it to be launched?</p></div>
		<div class="faq_text">
			<p>
				We're actively working on bringing LoveVeil to you. While we don't have an exact launch date
				yet, we'll keep you updated on our progress. Follow our social media for the latest news.
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(5)}>
		<div class="faq_title"><p>Will LoveVeil be free to use once it's launched?</p></div>
		<div class="faq_text">
			<p>
				Yes, LoveVeil is committed to making the core concept of prioritizing conversations and
				authentic connections absolutely free for all users. Our belief in meaningful connections
				drives us.
				<br /><br />
				To ensure it remains free, we rely on the generous support of our community. While our core features
				will always be accessible without charge, we may offer optional in-app purchases to unlock images
				faster. This way, you can enjoy a seamless experience while helping us keep LoveVeil accessible
				to everyone.
				<br /><br />
				We firmly believe that connections should be built on genuine conversations, not subscription
				fees. Your support and contributions are invaluable in making this vision a reality. Thank you
				for being a part of our mission to reshape online dating!
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(6)}>
		<div class="faq_title"><p>Is my data and privacy protected on LoveVeil?</p></div>
		<div class="faq_text">
			<p>
				Absolutely. We take your privacy seriously. LoveVeil is committed to safeguarding your data
				and ensuring a secure environment for meaningful connections. Your trust is our priority.
			</p>
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(7)}>
		<div class="faq_title"><p>How is Safety Ensured on LoveVeil?</p></div>
		<div class="faq_text">
			<p>
				Safety is our top priority at LoveVeil. We've implemented a comprehensive set of security
				measures to ensure a secure and enjoyable experience for all users. These measures include:
				<br /><br />
			</p>
			<ul>
				<li>
					<b>Profile Verification:</b> Users can verify their profiles to increase trust and authenticity
					within our community.
				</li>
				<li>
					<b>Moderation: </b> Our platform is actively monitored to identify and address any inappropriate
					content or behavior.
				</li>
				<li>
					<b> Privacy Controls:</b> You have control over your data and interactions, with robust privacy
					settings to protect your information.
				</li>
				<li>
					<b> Reporting System:</b> If you encounter any issues or concerns, our reporting system allows
					you to report and address them promptly.
				</li>
				<li>
					<b> Data Encryption:</b> All your data is encrypted to safeguard your privacy and personal
					information.
				</li>
				<li>
					<b>Community Guidelines:</b> LoveVeil has clear community guidelines that users are expected
					to follow to maintain a safe and respectful environment.
				</li>
				<li>
					<b> Ongoing Improvements:</b> We continually review and enhance our safety measures to adapt
					to evolving needs and challenges.
				</li>
			</ul>

			Your safety and security are of utmost importance to us.
		</div>
	</button>
	<button class="faq_container mini_hover2x faq_closed" on:click={() => getAllFaq(8)}>
		<div class="faq_title"><p>How can I get in contact?</p></div>
		<div class="faq_text">
			<p>
				We're here to assist you! Getting in touch with LoveVeil is easy. You can reach out to us
				through the following channels: <br /><br />
			</p>
			<ul>
				<li>
					<b>Email:</b>Feel free to email us directly at
					<a href="mailto:email@placeholder.com">email@placeholder.com</a> with any inquiries, feedback, or
					questions you may have.
				</li>
				<li>
					<b>Social Media:</b>Connect with us on our social media platforms, including Facebook,
					Twitter, and Instagram. We're active and responsive on these channels.
				</li>
			</ul>
		</div>
	</button>
</div>

<style lang="scss">
	h1 {
		font-size: 1.5rem;
		text-align: center;
		font-weight: 500;
		color: var(--primary-color-darker);
	}
	.faq_parent_container {
		@media screen and (min-width: 1000px) {
			padding: 2rem;
		}
		.faq_container {
			text-align: left;
			padding: 1.25rem 1rem;
			box-shadow: rgba(0, 0, 0, 0.1) 0px 1px 3px 0px, rgba(0, 0, 0, 0.06) 0px 1px 2px 0px;
			width: 100%;

			background: var(--faq-background);
			margin: 0.5rem 0;
		}
		.faq_title {
			font-weight: 400;
			font-size: 1.1rem;
		}
		.faq_text {
			background-color: var(--faq-background-darker);
			box-shadow: rgba(0, 0, 0, 0.05) 0px 1px 2px 0px;
			padding: 1rem;
			margin-top: 0.5rem;
			box-sizing: border-box;
			transition: all 250ms ease-out;
			line-height: 1.75;

			li:not(li:first-child) {
				margin: 1rem 0;
			}
		}
		.faq_closed .faq_text {
			padding: 0;
			margin-top: 0;
			max-height: 0;
			overflow: hidden;
		}
		a {
			color: var(--link-primary-color);
			font-weight: 500;
		}
	}
</style>
