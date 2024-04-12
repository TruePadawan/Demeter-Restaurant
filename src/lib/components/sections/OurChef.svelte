<script>
	import ChefImg from '$lib/images/chef.jpg';
</script>

<div
	class="flex flex-col gap-4 px-[2vw] py-[4vw] lg:flex-row lg:items-center lg:gap-x-[6vw] lg:px-[8vw] lg:py-[10vw]"
>
	<img src={ChefImg} alt="Chef Slavcho" class="max-h-[600px] object-cover lg:flex-1 object-top" />
	<div class="flex flex-col gap-2 lg:flex-1">
		<p class="text-3xl text-primary">A word from</p>
		<p class="text-5xl font-bold text-secondary">Our Chef</p>
		<p class="my-4 text-2xl text-primary">
			A peep at some distant orb has power to raise and purify our thoughts like a strain of sacred
			music, or a noble picture, or a passage from the grander poets. It always does one good.
		</p>
        <div>
            <p class="font-bold text-secondary text-2xl">Slavcho Karbashewski</p>
            <p class="text-primary text-xl mt-2">Head Chef</p>
        </div>
	</div>
</div>

<style>
	@media screen and (min-width: 1024px) {
		img {
			max-height: calc(100vh - 10vw);
		}
	}
</style>
