<script lang="ts">
	export let menuIsOpen: boolean;
</script>

<button class="flex flex-col items-end gap-y-1.5 md:hidden" on:click>
	<div class="bun h-0.5 w-6 bg-white"></div>
	<div class="bun h-0.5 w-6 bg-white {menuIsOpen ? 'w-4' : ''}"></div>
	<div class="bun h-0.5 w-6 bg-white {menuIsOpen ? 'w-2' : ''}"></div>
</button>

<style>
	.bun {
		transition: width 0.15s;
	}
</style>
