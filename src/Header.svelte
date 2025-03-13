<script>
	// @ts-nocheck

	import { page } from '$app/stores';
	import menu from '$lib/images/menu.svg';
	import icon from '$lib/images/icon.svg';

	let extra_header_open = false;

	import { clickOutside } from './clickOutside.ts';

	function handleClickOutside() {
		if (extra_header_open) extra_header_open = false;
	}
</script>

<header>
	<div class="main_header">
		<a
			href="/"
			class="{$page.url.pathname === '/'
				? 'active'
				: ''} mr-auto flex justify-center items-center mini_hover"
		>
			<img src={icon} alt="homepage icon for loveveil" class="w-10" /></a
		>
		<!--
		<a href="/about" class={$page.url.pathname === '/about' ? 'active' : ''}> About</a>
		<a href="/app" class={$page.url.pathname === '/app' ? 'active' : ''}> App</a>
		<a href="/blog" class={$page.url.pathname === '/blog' ? 'active' : ''}> Blog</a>
		<a href="/contact" class="{$page.url.pathname === '/contact' ? 'active' : ''} "> Contact</a>
		--->
		<a href="/" class="text-2xl header_title poetsenOne mini_hover">Loveveil</a>
		<a
			href="#0"
			class="ml-auto -scale-100 z-50 mini_hover"
			style="{extra_header_open
				? 'opacity:0;z-index:-99;'
				: 'opacity:1; z-index:100;'} transition: opacity 250ms ease-in-out"
			on:click={() => (extra_header_open = !extra_header_open)}
			><img src={menu} alt="Menu icon" /></a
		>
	</div>
	<nav
		class="extra_header z-40 flex flex-col text-left absolute right-0 h-full top-0 box-border {extra_header_open
			? 'opened'
			: 'closed'}"
		use:clickOutside
		on:click_outside={handleClickOutside}
	>
		<a
			href="/app"
			on:click={() => (extra_header_open = !extra_header_open)}
			class={$page.url.pathname === '/app' ? 'active' : ''}
		>
			Features</a
		>

		<a
			href="/about"
			on:click={() => (extra_header_open = !extra_header_open)}
			class={$page.url.pathname === '/about' ? 'active' : ''}
		>
			About Us</a
		>
		<a
			href="/faq"
			on:click={() => (extra_header_open = !extra_header_open)}
			class={$page.url.pathname === '/faq' ? 'active' : ''}
		>
			FAQ</a
		>
		<a
			href="/contact"
			on:click={() => (extra_header_open = !extra_header_open)}
			class={$page.url.pathname === '/contact' ? 'active' : ''}
		>
			Contact Us</a
		>
	</nav>
</header>

<style global lang="scss">
	.main_header {
		display: flex;
		flex-flow: row wrap;
		align-items: center;
		margin: 0.5rem;

		a {
			padding: 0.75rem 1.75rem;
			font-weight: 400;
			text-transform: capitalize;
			max-height: 4rem;
		}
	}

	.extra_header {
		transition: all 500ms ease-in-out;
		background: var(--background-primary-inverse);
		a {
			padding: 1.5rem 7rem;

			width: 100%;
			display: flex;
			align-items: center;
			justify-content: flex-start;
			color: var(--text-primary-inverse);
			font-weight: 300;
			background: var(--background-primary-inverse);
			&:hover {
				background: var(--background-primary-inverse-lighter);
				transition: background 250ms ease-in-out;
			}
		}
	}

	/*If extra_header closed*/

	:global(.closed) {
		/*width: 0vw;
		height: 0vh;
		overflow: hidden;
		*/
		transform: translateX(100%);
	}
	:global(.open) {
		width: 100vw;
		height: 100vh;
		transform: translateX(0%);
	}

	.active:not(.extra_header a) {
		color: var(--primary-color);
	}
</style>
