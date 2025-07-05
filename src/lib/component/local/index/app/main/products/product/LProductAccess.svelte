<script lang="ts">
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import PhosphorAndroidLogo from '$lib/component/library/phosphor/PhosphorAndroidLogo.svelte';
	import PhosphorAppleLogo from '$lib/component/library/phosphor/PhosphorAppleLogo.svelte';
	import PhosphorAppStoreLogo from '$lib/component/library/phosphor/PhosphorAppStoreLogo.svelte';
	import PhosphorFileArchive from '$lib/component/library/phosphor/PhosphorFileArchive.svelte';
	import PhosphorFiles from '$lib/component/library/phosphor/PhosphorFiles.svelte';
	import PhosphorGlobe from '$lib/component/library/phosphor/PhosphorGlobe.svelte';
	import PhosphorLinuxLogo from '$lib/component/library/phosphor/PhosphorLinuxLogo.svelte';
	import PhosphorWindowsLogo from '$lib/component/library/phosphor/PhosphorWindowsLogo.svelte';

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

<section id="product-stats" class="flex flex-col gap-4">
	<section id="available-platforms" class="flex">
		{#each product.accessLink as a}
			{#if a.link}
				{#key a.name}
					{@const Icon = getIconForPlatform(a.name)}
					<a
						href={a.link}
						target="_blank"
						title={a.name}
						class=" flex items-center gap-1"
					>
						<Icon />
					</a>
				{/key}
			{:else if a.platforms}
				{#each a.platforms as platform}
					{#key platform.name}
						{@const Icon = getIconForPlatform(platform.name)}
						<a
							href={platform.link}
							target="_blank"
							title={platform.name}
							class="flex items-center gap-1"
						>
							<Icon />
						</a>
					{/key}
				{/each}
			{/if}
		{/each}
	</section>
	<section id="access-button">
		<DaisyUiButton
			className="d-btn-primary d-btn-wide"
			onClick={() => {}}>Access</DaisyUiButton
		>
	</section>
</section>
