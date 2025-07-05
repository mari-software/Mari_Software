<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';

	let { productLine, i } = $props<{}>();
</script>

<section id="product-lines" class="flex flex-col gap-5">
	<h2 class="m-h2">Product Line - {i + 1}</h2>
	<div class=" grid grid-cols-2 gap-4">
		{#each productLine as product}
			<DaisyUiCard className="bg-primary-content px-3 pt-3 py-5">
				<figure class="size-20">
					<product.icon />
				</figure>
				<h3 class="m-h3">
					{product.name}
				</h3>
				<p>
					{product.description}
				</p>
			</DaisyUiCard>
		{/each}
	</div>
	<DaisyUiButton
		className="d-btn-primary w-auto self-center my-5"
		onClick={() => console.log()}
	>
		View More
	</DaisyUiButton>
</section>
