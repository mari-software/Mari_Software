<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCardBodyAction from '$lib/component/library/daisyui/card/body/action/DaisyUiCardBodyAction.svelte';
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
</script>

<section id="app-highlight">
	<DaisyUiCard className="bg-primary-content d-card-side py-3 px-1">
		<DaisyUiCardBody className="gap-2">
			<DaisyUiCardBodyTitle>
				<h1 class="m-h1">Product-Name</h1>
			</DaisyUiCardBodyTitle>
			<p>This is description.</p>
		</DaisyUiCardBody>
		<figure class="w-32 shrink-0 pr-5">
			<MariLogoSvg className="w-full h-auto" />
		</figure>
	</DaisyUiCard>
</section>
