<script>
	import EventsImg from '$lib/images/upcoming-events.jpg';
	import Button from '../Button.svelte';
</script>

<div id="events" class="flex flex-col gap-y-9 bg-[#333333] px-[2vw] py-[6vw] lg:px-[6vw] lg:py-[8vw]">
	<div class="text-center">
		<p class="text-2xl">Party with us!</p>
		<p class="mt-2 text-5xl font-bold">Upcoming Events</p>
	</div>
	<div class="flex flex-col lg:flex-row">
		<img src={EventsImg} alt="a group of people eating" class="max-h-96 object-cover lg:flex-1" />
		<div class="flex flex-col gap-4 bg-white px-[6%] py-[8%] lg:flex-1 lg:px-[4%] lg:py-[6%]">
			<div>
				<p class="text-2xl text-primary">Upcoming</p>
				<p class="text-4xl font-semibold text-secondary">Event Days</p>
			</div>
			<p class="text-primary">25 september, 2023</p>
			<p class="text-2xl text-primary">
				Apparently we had reached a great height in the atmosphere, for the sky was a dead black,
				and the stars had ceased to twinkle.
			</p>
			<Button className="lg:self-start">Book a table</Button>
		</div>
	</div>
</div>

<style>
	@media screen and (min-width: 1024px) {
		img {
			max-height: calc(100vh - 20vw);
		}
	}
</style>
