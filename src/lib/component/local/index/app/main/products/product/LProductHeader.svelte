<script lang="ts">
	import DaisyUiBadge from '$lib/component/library/daisyui/badge/DaisyUiBadge.svelte';

	let { product } = $props<{}>();
</script>

<section id="product-header" class="flex flex-col gap-5">
	<section id="header" class="flex justify-between gap-5">
		<figure>
			<product.icon className="size-26" />
		</figure>
		<section class="flex flex-col gap-3">
			<div>
				<h1 class="m-h1">{product.name}</h1>
				<p class="text-sm opacity-50">{product.groupName}</p>
			</div>
			<p class="line-clamp-2 text-sm">{product.description}</p>
		</section>
	</section>
	<section id="category" class="flex justify-end gap-3">
		{#each product.category as c}
			<DaisyUiBadge className="d-badge-neutral d-badge-outline"
				>{c}</DaisyUiBadge
			>
		{/each}
	</section>
</section>
