<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';

	let { product } = $props<{}>();
</script>

<section id="similar-product" class="flex flex-col gap-5">
	<h3 class="m-h3">Similar Products</h3>
	<div class=" grid grid-cols-2 gap-4">
		{#each product.similarProduct as p}
			<DaisyUiCard className="bg-primary-content px-3 pt-3 py-5">
				<figure class="size-20">
					<p.icon />
				</figure>
				<h3 class="m-h3">
					{p.name}
				</h3>
				<p>
					{p.description}
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
