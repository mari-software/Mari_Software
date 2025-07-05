<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';

	let { articleLines } = $props<{}>();
</script>

<section id="articles" class="flex flex-col gap-5">
	<h2 class="m-h2">Articles</h2>
	<div class=" grid grid-cols-2 gap-4">
		{#each articleLines as article}
			<DaisyUiCard className="bg-primary-content gap-3 py-10 px-5">
				<h3 class="m-h3">
					{article.title}
				</h3>
				<p>
					{article.description}
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
