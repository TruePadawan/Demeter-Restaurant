<script lang="ts">
	import '../app.css';
	import MenuButton from '$lib/components/MenuButton.svelte';
	import Hero from '$lib/components/sections/Hero.svelte';
	import History from '$lib/components/sections/History.svelte';
	import SpecialMeals from "$lib/components/sections/SpecialMeals.svelte";

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
		: ''} absolute flex h-screen w-screen flex-col gap-4 bg-[#333333]/80 px-6 pt-6"
>
	<div class="self-end">
		<MenuButton {menuIsOpen} on:click={closeMenu} />
	</div>
	<div class="flex flex-col items-center gap-5 text-xl font-light text-white">
		<a href="#about-us" class="nav-link">About Us</a>
		<a href="#special-meals" class="nav-link">Menu</a>
		<a href="#events" class="nav-link">Events</a>
		<a href="#news" class="nav-link">News</a>
		<a href="#contact" class="nav-link">Contact</a>
		<hr class="w-full" />
		<a href="#book-a-table" class="nav-link">Book a table</a>
		<a href="#see-menu" class="nav-link">See Menu</a>
	</div>
</div>
<Hero {menuIsOpen} on:menubtnclicked={openMenu} />
<History />
<SpecialMeals />

<style>
	:global(body) {
		font-family: 'Rethink Sans', sans-serif;
		margin: 0;
		color: white;
		height: 100vh;
	}
</style>
