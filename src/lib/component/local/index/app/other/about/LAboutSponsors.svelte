<script lang="ts">
	let { dummyData } = $props<{}>();
</script>

<section id="sponsors">
	<h3 class="m-h3">Sponsors</h3>
	<section id="collaborating-units" class="mt-5 grid grid-cols-2">
		{#each dummyData as unit}
			<div class="flex">
				<figure class="size-20">
					<unit.icon className="size-14" />
				</figure>
				{unit.name}
			</div>
		{/each}
	</section>
</section>
