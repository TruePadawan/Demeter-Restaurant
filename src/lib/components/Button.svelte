<script lang="ts">
	export let outlined = false;
	export let type: 'button' | 'submit' = 'button';
	export let className = '';
</script>

<button
	{type}
	class="rounded px-8 py-3 text-lg {outlined
		? 'border border-white/40 hover:bg-white/40'
		: 'bg-[#f59d29] hover:bg-[#f59d29cc]'} {className}"
>
	<slot />
</button>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

	button {
		font-family: 'Montserrat', sans-serif;
		transition: background-color 0.5s;
	}
</style>
