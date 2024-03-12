<script lang="ts">
	import '../app.css';
	import logo from '$lib/images/logo.png';
	import Button from '$lib/components/Button.svelte';
</script>

<div class="hero flex flex-col">
	<nav class="py-5 px-32 flex items-center justify-between">
		<a class="no-underline flex gap-x-1 items-center" href="/">
			<img class="logo" src={logo} alt="demeter logo" />
			<span class="text-white text-4xl font-bold">DEMETER</span>
		</a>
		<div class="flex gap-x-10 text-xl text-white font-light">
			<a href="#about-us" class="nav-link">About Us</a>
			<a href="#menu" class="nav-link">Menu</a>
			<a href="#events" class="nav-link">Events</a>
			<a href="#news" class="nav-link">News</a>
			<a href="#contact" class="nav-link">Contact</a>
		</div>
	</nav>
	<div class="grow flex flex-col justify-center px-36">
		<div>
			<p class="text-7xl font-bold">For Fine Dine</p>
			<p class="text-6xl font-light">Best Place, Best Service</p>
		</div>
		<p class="my-8 font-light text-3xl">We will be happy to see you in our restaurant</p>
		<div class="flex gap-x-8">
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
		background-image: url('$lib/images/hero-section.jpg');
		background-size: cover;
		height: 100vh;
	}

	.logo {
		width: auto;
		height: 28px;
	}
</style>
