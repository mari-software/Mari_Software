<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiDrawerContent from '$lib/component/library/daisyui/drawer/content/DaisyUiDrawerContent.svelte';
	import DaisyUiDrawer from '$lib/component/library/daisyui/drawer/DaisyUiDrawer.svelte';
	import DaisyUiDrawerSide from '$lib/component/library/daisyui/drawer/side/DaisyUiDrawerSide.svelte';
	import DaisyUiDrawerToggle from '$lib/component/library/daisyui/drawer/toggle/DaisyUiDrawerToggle.svelte';
	import DaisyUiNavbarCenter from '$lib/component/library/daisyui/navbar/center/DaisyUiNavbarCenter.svelte';
	import DaisyUiNavbar from '$lib/component/library/daisyui/navbar/DaisyUiNavbar.svelte';
	import DaisyUiNavbarEnd from '$lib/component/library/daisyui/navbar/end/DaisyUiNavbarEnd.svelte';
	import DaisyUiNavbarStart from '$lib/component/library/daisyui/navbar/start/DaisyUiNavbarStart.svelte';
	import DaisyUiStatus from '$lib/component/library/daisyui/status/DaisyUiStatus.svelte';
	import LucideBell from '$lib/component/library/lucide/LucideBell.svelte';
	import LucideMenu from '$lib/component/library/lucide/LucideMenu.svelte';
	import LucideSearch from '$lib/component/library/lucide/LucideSearch.svelte';
	import { goToRoute } from '$lib/util/sveltekit/router.sveltekit.util';
	import GIndexDrawerContent from './GIndexDrawerContent.svelte';
</script>

<DaisyUiNavbar className="bg-base-200 shadow-md px-5">
	<DaisyUiNavbarStart>
		<DaisyUiDrawer>
			<DaisyUiDrawerToggle drawerName="main-drawer" />

			<DaisyUiDrawerContent
				drawerName="main-drawer"
				className="d-btn-square"
			>
				<LucideMenu />
			</DaisyUiDrawerContent>
			<DaisyUiDrawerSide
				drawerName="main-drawer"
				drawerClassName="w-72"
			>
				<!-- Drawer Content -->
				<GIndexDrawerContent />
			</DaisyUiDrawerSide>
		</DaisyUiDrawer>
	</DaisyUiNavbarStart>

	<DaisyUiNavbarCenter>
		<a href="/" class="d-btn d-btn-ghost text-xl">
			<MariLogoSvg className="size-10" />
		</a>
	</DaisyUiNavbarCenter>

	<DaisyUiNavbarEnd>
		<DaisyUiButton
			className="d-btn-ghost d-btn-circle"
			onClick={() => console.log('Heloo')}
		>
			<LucideSearch />
		</DaisyUiButton>

		<DaisyUiStatus className="d-status-primary" effect="ping">
			<DaisyUiButton
				className="d-btn-ghost d-btn-circle"
				onClick={() => goToRoute('/app/other/notification')}
			>
				<LucideBell />
			</DaisyUiButton>
		</DaisyUiStatus>
	</DaisyUiNavbarEnd>
</DaisyUiNavbar>
