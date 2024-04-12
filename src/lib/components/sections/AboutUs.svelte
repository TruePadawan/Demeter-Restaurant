<script>
	import NYTimesLogo from '$lib/images/logo/nytimes.svg';
	import TheGuardianLogo from '$lib/images/logo/theguardian.png';
	import WSJLogo from '$lib/images/logo/wsj.svg';
</script>

<div
	id="about-us"
	class="mt-4 flex flex-col gap-y-9 bg-[#333333] px-[2vw] py-[6vw] lg:px-[6vw] lg:py-[8vw]"
>
	<div class="text-center">
		<p class="text-2xl">Press</p>
		<p class="mt-2 font-['Platypi'] text-5xl font-semibold">About Us</p>
	</div>
	<div class="grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-3 2xl:gap-8">
		<div class="flex flex-col gap-y-6 rounded-sm bg-white p-10">
			<img src={NYTimesLogo} alt="New York Times" />
			<p class="text-2xl leading-relaxed text-primary">
				"Apparently we had reached a great height in the atmosphere, for the sky was a dead black,
				and the stars had ceased to twinkle. By the same illusion which lifts the horizon of the sea
				to the level."
			</p>
			<p class="mt-auto font-['Platypi'] text-2xl font-semibold text-black">The New York Times</p>
		</div>
		<div class="flex flex-col gap-y-6 rounded-sm bg-white p-10">
			<img src={TheGuardianLogo} alt="The Guardian" />
			<p class="text-2xl leading-relaxed text-primary">
				"Apparently we had reached a great height in the atmosphere, for the sky was a dead black,
				and the stars had ceased to twinkle. By the same illusion which lifts the horizon of the sea
				to the level."
			</p>
			<p class="mt-auto font-['Platypi'] text-2xl font-semibold text-black">The Guardian</p>
		</div>
		<div class="flex flex-col gap-y-6 rounded-sm bg-white p-10">
			<img src={WSJLogo} alt="Wall Street Journal" />
			<p class="text-2xl leading-relaxed text-primary">
				"Apparently we had reached a great height in the atmosphere, for the sky was a dead black,
				and the stars had ceased to twinkle. By the same illusion which lifts the horizon of the sea
				to the level."
			</p>
			<p class="mt-auto font-['Platypi'] text-2xl font-semibold text-black">
				The Wall Street Journal
			</p>
		</div>
	</div>
</div>
