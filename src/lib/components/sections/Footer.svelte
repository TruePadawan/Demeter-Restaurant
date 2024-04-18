<script>
	import logo from '$lib/images/logo/logo.png';
	import IconBrandFacebookFilled from '@tabler/icons-svelte/IconBrandFacebookFilled.svelte';
	import IconBrandInstagram from '@tabler/icons-svelte/IconBrandInstagram.svelte';
	import IconBrandTwitterFilled from '@tabler/icons-svelte/IconBrandTwitterFilled.svelte';
</script>

<div class="flex flex-col items-center bg-[#333333] px-2 pb-24 pt-12">
	<a class="flex flex-col items-center gap-1 no-underline" href="/">
		<img class="h-7 w-auto" src={logo} alt="demeter logo" />
		<span class="company-name text-4xl font-medium text-white">DEMETER</span>
	</a>
	<div class="mt-14 flex gap-8">
		<a href="#about-us">About Us</a>
		<a href="#special-meals">Menu</a>
		<a href="#events">Events</a>
		<a href="#news">News</a>
		<a href="#reserve-table">Contact</a>
	</div>
	<div class="mt-20 flex gap-2">
		<div class="rounded-full border border-white p-3">
			<IconBrandFacebookFilled />
		</div>
		<div class="rounded-full border border-white p-3">
			<IconBrandTwitterFilled />
		</div>
		<div class="rounded-full border border-white p-3">
			<IconBrandInstagram />
		</div>
	</div>
	<p class="mt-8 text-center text-xl">2023 DEMETER Restaurant. All Rights Reserved.</p>
</div>
