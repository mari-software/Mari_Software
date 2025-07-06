<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiCardBodyAction from '$lib/component/library/daisyui/card/body/action/DaisyUiCardBodyAction.svelte';
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
	import { goToRoute } from '$lib/util/sveltekit/router.sveltekit.util';
</script>

<section id="app-hero">
	<DaisyUiCard className="bg-primary-content d-card-side py-3 px-1">
		<DaisyUiCardBody className="gap-5">
			<DaisyUiCardBodyTitle>
				<h1 class="m-h1">
					<span class="text-primary">MARI</span> has whatever you need
				</h1>
			</DaisyUiCardBodyTitle>
			<DaisyUiCardBodyAction>
				<DaisyUiButton
					className="d-btn-primary m-h4"
					onClick={() => goToRoute('/app/main/categories')}
				>
					See More
				</DaisyUiButton>
			</DaisyUiCardBodyAction>
		</DaisyUiCardBody>
		<figure class="w-32 shrink-0 pr-5">
			<MariLogoSvg className="w-full h-auto" />
		</figure>
	</DaisyUiCard>
</section>
