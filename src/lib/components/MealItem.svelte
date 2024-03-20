<script lang="ts">
	export let name: string;
	export let extraInfo: string;
	export let price: number;
</script>

<li class="flex justify-between text-[#6e6e6a]">
	<div class="flex flex-col gap-1">
		<p class="text-xl font-medium">{name}</p>
		<p class="font-thin">{extraInfo}</p>
	</div>
	<p class="text-xl">${price.toFixed(2)}</p>
</li>
