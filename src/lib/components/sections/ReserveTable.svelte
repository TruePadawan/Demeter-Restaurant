<script>
	import Button from '$lib/components/Button.svelte';
	import ReserveSectionImg from '$lib/images/reservations.jpg';
</script>

<div
	id="reserve-table"
	class="mt-4 flex flex-col gap-4 px-[2vw] py-[4vw] lg:flex-row lg:items-center lg:gap-x-[6vw] lg:px-[8vw] lg:py-[10vw]"
>
	<div class="flex-1">
		<div>
			<p class="text-3xl text-primary">A Table</p>
			<p class="mt-2 text-5xl font-bold text-secondary">Reserve</p>
		</div>
		<form class="mt-11 flex flex-col gap-8">
			<div>
				<label for="reserve-date">DATE</label>
				<input type="date" id="reserve-date" class="text-primary" />
			</div>
			<div>
				<label for="reserve-time">TIME</label>
				<input type="time" id="reserve-time" class="text-primary" />
			</div>
			<div class="flex flex-col gap-2">
				<label for="reserve-guests">GUESTS</label>
				<select id="reserve-guests" class="text-primary">
					<option>1 person</option>
					<option>2 people</option>
					<option>3 people</option>
					<option>4 people</option>
					<option>5 people</option>
					<option>6 people</option>
				</select>
			</div>
			<Button className="lg:self-start mt-7">Find a table</Button>
		</form>
	</div>
	<img
		src={ReserveSectionImg}
		alt="two glasses of wine"
		class="max-h-[600px] object-cover lg:flex-1"
	/>
</div>

<style>
	form > div {
		display: flex;
		flex-direction: column;
		row-gap: 0.5rem;
	}

	input,
	select {
		background-color: transparent;
		padding: 8px 4px;
		width: 100%;
		border: 1px solid rgba(128, 128, 128, 0.582);
		border-radius: 6px;
	}

	label {
		color: rgb(51, 51, 52);
		font-weight: bold;
	}
</style>
