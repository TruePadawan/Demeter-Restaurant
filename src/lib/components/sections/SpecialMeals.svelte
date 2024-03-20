<script>
	import SpecialMealsImg from '$lib/images/special-meals.jpg';
	import MealItem from '$lib/components/MealItem.svelte';
</script>

<div
	id="special-meals"
	class="mt-4 flex flex-col gap-4 px-[2vw] py-[4vw] lg:h-screen lg:flex-row lg:items-center lg:gap-x-[6vw] lg:px-[8vw] lg:py-[10vw]"
>
	<div class="flex flex-col gap-2 lg:flex-1">
		<p class="text-3xl font-light text-[#6e6e6a]">Check out our</p>
		<p class="text-5xl font-medium text-[#333334]">Special Meals</p>
		<ul class="mt-12 flex flex-col gap-6">
			<MealItem
				name="Fish & Chips"
				extraInfo="Served with soy sauce, wasabi, pickled ginger and chopsticks"
				price={14.0}
			/>
			<MealItem
				name="Fishermen's Basket"
				extraInfo="Snow crab, avocado, cucumber, tobiko, Japanese mayonnaise"
				price={7}
			/>
			<MealItem
				name="Chicken Breast Saute Sec"
				extraInfo="A Latte is a coffe drink made with espresso and steamed milk"
				price={5}
			/>
			<MealItem
				name="Crisp Pork Belly"
				extraInfo="Candied salmon, basil potato puree, baby kale marsala"
				price={18}
			/>
		</ul>
	</div>
	<img
		src={SpecialMealsImg}
		alt="hands picking at food"
		class="max-h-96 w-full object-cover lg:flex-1"
	/>
</div>

<style>
	@media screen and (min-width: 1024px) {
		img {
			max-height: calc(100vh - 20vw);
		}
	}
</style>
