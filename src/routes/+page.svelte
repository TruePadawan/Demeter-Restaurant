<script lang="ts">
	import '../app.css';
	import logo from '$lib/images/logo.png';
	import Button from '$lib/components/Button.svelte';
	import MenuButton from '$lib/components/MenuButton.svelte';

	let menuIsOpen = false;

	function openMenu() {
		menuIsOpen = true;
	}

	function closeMenu() {
		menuIsOpen = false;
	}
</script>

<div
	class="{!menuIsOpen
		? 'hidden'
		: ''} absolute flex h-screen w-screen flex-col gap-4 bg-[#333333]/80 px-6 pt-6"
>
	<div class="self-end">
		<MenuButton {menuIsOpen} on:click={closeMenu} />
	</div>
	<div class="flex flex-col items-center gap-5 text-xl font-light text-white">
		<a href="#about-us" class="nav-link">About Us</a>
		<a href="#menu" class="nav-link">Menu</a>
		<a href="#events" class="nav-link">Events</a>
		<a href="#news" class="nav-link">News</a>
		<a href="#contact" class="nav-link">Contact</a>
		<hr class="w-full" />
		<a href="#book-a-table" class="nav-link">Book a table</a>
		<a href="#see-menu" class="nav-link">See Menu</a>
	</div>
</div>
<div class="hero flex flex-col bg-center xl:bg-top">
	<nav class="flex items-center justify-between px-6 pt-3 lg:px-32 lg:pt-5">
		<a class="flex items-center gap-x-1 no-underline" href="/">
			<img class="logo" src={logo} alt="demeter logo" />
			<span class="company-name text-4xl font-bold text-white">DEMETER</span>
		</a>
		<div class="hidden gap-x-10 text-xl font-light text-white md:flex">
			<a href="#about-us" class="nav-link">About Us</a>
			<a href="#menu" class="nav-link">Menu</a>
			<a href="#events" class="nav-link">Events</a>
			<a href="#news" class="nav-link">News</a>
			<a href="#contact" class="nav-link">Contact</a>
		</div>
		<MenuButton {menuIsOpen} on:click={openMenu} />
	</nav>
	<div class="hero-main flex grow flex-col justify-end md:justify-center">
		<div>
			<p class="text-7xl font-bold">For Fine Dine</p>
			<p class="text-6xl font-light">Best Place, Best Service</p>
		</div>
		<p class="my-8 text-3xl font-light">We will be happy to see you in our restaurant</p>
		<div class="hidden flex-col gap-x-8 gap-y-2 sm:flex-row md:flex">
			<Button>Book a table</Button>
			<Button outlined>See menu</Button>
		</div>
	</div>
</div>

<style>
	:global(body) {
		font-family: 'Korolev', sans-serif;
		margin: 0;
		color: white;
		height: 100vh;
	}

	.hero {
		/** Darken background image */
		background-image: linear-gradient(rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.25)),
			url('$lib/images/hero-section.jpg');
		background-size: cover;
		height: 100vh;
	}

	.logo {
		width: auto;
		height: 28px;
	}

	.hero-main {
		padding: 0 3vw;
	}

	@media screen and (min-width: 640px) {
		.hero-main {
			padding: 0 10vw;
		}
	}

	/* not sure why there is some odd space on mobile, this is a quick fix for it */
	/* @media screen and (max-width: 400px) {
		.company-name {
			height: 34px;
		}
	} */
</style>
