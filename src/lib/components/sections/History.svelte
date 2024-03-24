<script>
	import HistorySectionImg from '$lib/images/history-section.jpg';
	import Button from '$lib/components/Button.svelte';
</script>

<div
	id="about-us"
	class="flex flex-col gap-4 px-[2vw] py-[4vw] lg:flex-row lg:items-center lg:gap-x-[6vw] lg:px-[8vw] lg:py-[10vw]"
>
	<img src={HistorySectionImg} alt="demeter restaurant" class="max-h-96 object-cover lg:flex-1" />
	<div class="flex flex-col gap-2 lg:flex-1">
		<p class="text-3xl text-[#6e6e6a]">Discover</p>
		<p class="text-5xl font-semibold text-[#333334]">Our History</p>
		<p class="my-4 text-2xl text-[#6e6e6a]">
			A peep at some distant orb has power to raise and purify our thoughts like a strain of sacred
			music, or a noble picture, or a passage from the grander poets. It always does one good.
		</p>
		<Button className="lg:self-start">Read more</Button>
	</div>
</div>

<style>
	@media screen and (min-width: 1024px) {
		img {
			max-height: calc(100vh - 20vw);
		}
	}
</style>
