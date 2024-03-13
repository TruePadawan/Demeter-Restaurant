<script lang="ts">
	import '../app.css';
	import logo from '$lib/images/logo.png';
	import Button from '$lib/components/Button.svelte';
	import { IconMenu2 } from '@tabler/icons-svelte';
</script>

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
		<button class="md:hidden">
			<IconMenu2 stroke={2} />
		</button>
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
		background-image: url('$lib/images/hero-section.jpg');
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
