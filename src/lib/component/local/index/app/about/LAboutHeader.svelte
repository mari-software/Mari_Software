<script>
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
</script>

<section id="header" class="flex flex-col gap-2">
	<h1 class="m-h1">About <span class="text-primary">MARI</span></h1>
	<DaisyUiCard className="bg-primary-content d-card-side py-3 px-1">
		<DaisyUiCardBody>
			<DaisyUiCardBodyTitle>
				<h1>
					This is the <span class="text-primary">image example</span> for
					About Us.
				</h1>
			</DaisyUiCardBodyTitle>
		</DaisyUiCardBody>
		<figure class="w-32 shrink-0 pr-5">
			<MariLogoSvg className="w-full h-auto" />
		</figure>
	</DaisyUiCard>
</section>
