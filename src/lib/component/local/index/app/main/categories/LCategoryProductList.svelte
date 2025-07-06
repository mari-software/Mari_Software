<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
	import DaisyUiLink from '$lib/component/library/daisyui/link/DaisyUiLink.svelte';

	let { dummyData } = $props<{}>();
</script>

<section class="flex flex-col gap-5">
	<h3 class="m-h3">Category Header</h3>

	<section class="flex flex-col gap-5">
		{#each dummyData as p}
			<DaisyUiLink
				href="/app/main/products/1"
				className="no-underline"
			>
				<DaisyUiCard
					className="d-card-side bg-primary-content py-3 px-5"
				>
					<figure class="w-24 shrink-0">
						<p.icon className="w-full h-auto" />
					</figure>
					<DaisyUiCardBody>
						<DaisyUiCardBodyTitle>
							{p.name}
						</DaisyUiCardBodyTitle>
						<p>
							{p.description}
						</p>
					</DaisyUiCardBody>
				</DaisyUiCard>
			</DaisyUiLink>
		{/each}
	</section>
</section>
