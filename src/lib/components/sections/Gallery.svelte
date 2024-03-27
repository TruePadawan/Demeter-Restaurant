<script>
	import Interior1 from '$lib/images/interior-1.jpg';
	import Interior2 from '$lib/images/interior-2.jpg';
	import Interior3 from '$lib/images/interior-3.jpg';
	import Interior4 from '$lib/images/interior-4.jpg';
	import Interior5 from '$lib/images/interior-5.jpg';
	import Interior6 from '$lib/images/interior-6.jpg';
</script>

<div class="mt-4 flex flex-col gap-y-9 px-[2vw] py-[6vw] lg:px-[6vw] lg:py-[8vw]">
	<div class="text-center">
		<p class="text-2xl text-primary">Gallery</p>
		<p class="mt-2 text-5xl font-bold text-secondary">Our Interior</p>
	</div>
	<div class="grid grid-cols-1 gap-6 sm:grid-cols-2 md:grid-cols-3">
		<img class="h-full max-h-80 w-full object-cover" src={Interior1} alt="interior" />
		<img class="h-full max-h-80 w-full object-cover" src={Interior2} alt="interior" />
		<img class="h-full max-h-80 w-full object-cover" src={Interior3} alt="interior" />
		<img class="h-full max-h-80 w-full object-cover" src={Interior4} alt="interior" />
		<img class="h-full max-h-80 w-full object-cover" src={Interior5} alt="interior" />
		<img class="h-full max-h-80 w-full object-cover" src={Interior6} alt="interior" />
	</div>
</div>
