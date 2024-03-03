<script>
	import '../app.css';
	import logo from '$lib/images/logo.png';
</script>

<div class="hero">
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
</div>

<style>
	:global(body) {
		font-family: 'Korolev Light', sans-serif;
		margin: 0;
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
