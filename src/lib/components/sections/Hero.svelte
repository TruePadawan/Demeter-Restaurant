<script>
	import logo from '$lib/images/logo.png';
	import Button from '../Button.svelte';
	import MenuButton from '../MenuButton.svelte';
	import { createEventDispatcher } from 'svelte';

	export let menuIsOpen = false;

	const dispatch = createEventDispatcher();

	function dispatchClickEvent() {
		dispatch('menubtnclicked');
	}
</script>

<div class="hero flex h-screen flex-col bg-cover bg-center xl:bg-top">
	<nav class="flex items-center justify-between px-6 pt-3 lg:px-32 lg:pt-5">
		<a class="flex items-center gap-x-1 no-underline" href="/">
			<img class="h-7 w-auto" src={logo} alt="demeter logo" />
			<span class="company-name text-4xl font-medium text-white">DEMETER</span>
		</a>
		<div class="hidden gap-x-10 text-xl font-light text-white md:flex">
			<a href="#about-us" class="nav-link">About Us</a>
			<a href="#special-meals" class="nav-link">Menu</a>
			<a href="#events" class="nav-link">Events</a>
			<a href="#news" class="nav-link">News</a>
			<a href="#contact" class="nav-link">Contact</a>
		</div>
		<MenuButton {menuIsOpen} on:click={dispatchClickEvent} />
	</nav>
	<div class="hero-main flex grow flex-col justify-end px-[3vw] md:justify-center md:px-[10vw]">
		<div>
			<p class="text-7xl font-bold">For Fine Dine</p>
			<p class="text-6xl">Best Place, Best Service</p>
		</div>
		<p class="my-8 text-3xl">We will be happy to see you in our restaurant</p>
		<div class="hidden flex-col gap-x-8 gap-y-2 sm:flex-row md:flex">
			<Button>Book a table</Button>
			<Button outlined>See menu</Button>
		</div>
	</div>
</div>

<style>
	.hero {
		/** Darken background image */
		background-image: linear-gradient(rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.25)),
			url('$lib/images/hero-section.jpg');
	}

	.company-name {
		font-family: 'Korolev', sans-serif;
	}
</style>
