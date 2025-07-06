<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiTooltip from '$lib/component/library/daisyui/tooltip/DaisyUiTooltip.svelte';
	import LucideHeart from '$lib/component/library/lucide/LucideHeart.svelte';
	import LucideShare2 from '$lib/component/library/lucide/LucideShare2.svelte';
	import PhosphorAndroidLogo from '$lib/component/library/phosphor/PhosphorAndroidLogo.svelte';
	import PhosphorAppleLogo from '$lib/component/library/phosphor/PhosphorAppleLogo.svelte';
	import PhosphorAppStoreLogo from '$lib/component/library/phosphor/PhosphorAppStoreLogo.svelte';
	import PhosphorFileArchive from '$lib/component/library/phosphor/PhosphorFileArchive.svelte';
	import PhosphorFiles from '$lib/component/library/phosphor/PhosphorFiles.svelte';
	import PhosphorGlobe from '$lib/component/library/phosphor/PhosphorGlobe.svelte';
	import PhosphorLinuxLogo from '$lib/component/library/phosphor/PhosphorLinuxLogo.svelte';
	import PhosphorWindowsLogo from '$lib/component/library/phosphor/PhosphorWindowsLogo.svelte';
	import { goToRoute } from '$lib/util/sveltekit/router.sveltekit.util';

	function getIconForPlatform(name: string) {
		switch (name.toLowerCase()) {
			case 'website':
				return PhosphorGlobe;
			case 'file':
				return PhosphorFiles;
			case 'source code':
				return PhosphorFileArchive;
			case 'window':
				return PhosphorWindowsLogo;
			case 'macos':
				return PhosphorAppleLogo;
			case 'ios':
				return PhosphorAppStoreLogo;
			case 'linux':
				return PhosphorLinuxLogo;
			case 'android':
				return PhosphorAndroidLogo;
			default:
				return null;
		}
	}

	let { product } = $props<{}>();
</script>

<section id="product-stats" class="flex w-full flex-col gap-3">
	<!-- Platform icons section -->
	<section>
		<h3 class="m-h3">Available Platforms</h3>
		<p class="opacity-50">click icons to access ...</p>
	</section>
	<section
		id="available-platforms"
		class="grid w-full grid-cols-6 gap-3 p-2"
	>
		{#each product.accessLink as a}
			{#if a.link}
				{#key a.name}
					{@const Icon = getIconForPlatform(a.name)}
					<DaisyUiButton
						className="d-btn-square size-12"
						onClick={() => goToRoute(a.link as string)}
					>
						<DaisyUiTooltip
							className="d-tooltip-top d-alert-info"
							tooltipText={a.name}
						>
							<Icon />
						</DaisyUiTooltip>
					</DaisyUiButton>
				{/key}
			{:else if a.platforms}
				{#each a.platforms as platform}
					{#key platform.name}
						{@const Icon = getIconForPlatform(platform.name)}
						<DaisyUiButton
							className="d-btn-square size-12"
							onClick={() => goToRoute(product.link as string)}
						>
							<DaisyUiTooltip
								className="d-tooltip-top d-alert-info"
								tooltipText={platform.name}
							>
								<Icon />
							</DaisyUiTooltip>
						</DaisyUiButton>
					{/key}
				{/each}
			{/if}
		{/each}
	</section>

	<section>
		<h3 class="m-h3">Bookmarks</h3>
	</section>
	<section class="flex justify-between">
		<div class="flex gap-3">
			<DaisyUiButton onClick={() => console.log()}>
				<LucideShare2 className="size-7" /> Share to others
			</DaisyUiButton>
		</div>
		<div class="flex gap-3">
			<DaisyUiButton onClick={() => console.log()}>
				<LucideHeart className="size-7" /> Add to wishlist
			</DaisyUiButton>
		</div>
	</section>
</section>
