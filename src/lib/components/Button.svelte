<script lang="ts">
	export let outlined = false;
	export let type: 'button' | 'submit' = 'button';
</script>

<button
	{type}
	class="px-8 py-3 text-lg rounded {outlined
		? 'border border-white/40 hover:bg-white/40'
		: 'bg-[#f99118] hover:bg-[#f99018ce]'}"
>
	<slot />
</button>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

	button {
		font-family: 'Montserrat', sans-serif;
	}
</style>
