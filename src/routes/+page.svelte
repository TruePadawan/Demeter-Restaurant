<script lang="ts">
	import '../app.css';
	import MenuButton from '$lib/components/MenuButton.svelte';
	import Hero from '$lib/components/sections/Hero.svelte';
	import History from '$lib/components/sections/History.svelte';
	import SpecialMeals from '$lib/components/sections/SpecialMeals.svelte';
	import UpcomingEvents from '$lib/components/sections/UpcomingEvents.svelte';

	let menuIsOpen = false;

	function openMenu() {
		menuIsOpen = true;
	}

	function closeMenu() {
		menuIsOpen = false;
	}
</script>

<!-- MOBILE HAMBURGER MENU -->
<div
	class="{!menuIsOpen
		? 'hidden'
		: ''} fixed flex h-screen w-screen flex-col gap-4 bg-[#333333]/80 px-6 pt-6"
>
	<div class="self-end">
		<MenuButton {menuIsOpen} on:click={closeMenu} />
	</div>
	<div class="flex flex-col items-center gap-5 text-xl font-light text-white">
		<a href="#about-us">About Us</a>
		<a href="#special-meals">Menu</a>
		<a href="#events">Events</a>
		<a href="#news">News</a>
		<a href="#contact">Contact</a>
		<hr class="w-full" />
		<a href="#book-a-table">Book a table</a>
		<a href="#see-menu">See Menu</a>
	</div>
</div>
<Hero {menuIsOpen} on:menubtnclicked={openMenu} />
<History />
<SpecialMeals />
<UpcomingEvents />

<style>
	:global(body) {
		font-family: 'Rethink Sans', sans-serif;
		margin: 0;
		color: white;
		height: 100vh;
	}
</style>
