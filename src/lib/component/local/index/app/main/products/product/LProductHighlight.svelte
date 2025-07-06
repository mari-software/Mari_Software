<script lang="ts">
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';

	let { product } = $props<{}>();
</script>

<section id="highlight">
	<DaisyUiCard
		className="bg-primary-content d-card-side py-3 px-1 min-h-52"
	>
		<DaisyUiCardBody className="gap-5">
			<DaisyUiCardBodyTitle>
				<h2 class="m-h2">
					This is the <span class="text-primary">screenshot</span> section
					of the product.
				</h2>
			</DaisyUiCardBodyTitle>
		</DaisyUiCardBody>
		<figure class="w-32 shrink-0 pr-5">
			<product.icon className="w-full h-auto" />
		</figure>
	</DaisyUiCard>
</section>
