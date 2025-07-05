<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiAvatar from '$lib/component/library/daisyui/avatar/DaisyUiAvatar.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiMenu from '$lib/component/library/daisyui/menu/DaisyUiMenu.svelte';
	import DaisyUiNavbarCenter from '$lib/component/library/daisyui/navbar/center/DaisyUiNavbarCenter.svelte';
	import DaisyUiNavbar from '$lib/component/library/daisyui/navbar/DaisyUiNavbar.svelte';
	import DaisyUiNavbarEnd from '$lib/component/library/daisyui/navbar/end/DaisyUiNavbarEnd.svelte';
	import DaisyUiNavbarStart from '$lib/component/library/daisyui/navbar/start/DaisyUiNavbarStart.svelte';
	import DaisyUiStatus from '$lib/component/library/daisyui/status/DaisyUiStatus.svelte';
	import LucideBell from '$lib/component/library/lucide/LucideBell.svelte';
	import LucideMenu from '$lib/component/library/lucide/LucideMenu.svelte';
	import LucideSearch from '$lib/component/library/lucide/LucideSearch.svelte';
	import { goToRoute } from '$lib/util/sveltekit/router.sveltekit.util';
</script>

<DaisyUiNavbar className="bg-base-200 shadow-md px-5">
	<DaisyUiNavbarStart>
		<div class="d-drawer">
			<input id="my-drawer" type="checkbox" class="d-drawer-toggle" />
			<div class="d-drawer-content">
				<!-- Page content here -->
				<label for="my-drawer" class="d-btn-ghost d-btn-circle"
					><LucideMenu />
				</label>
			</div>
			<div class="d-drawer-side">
				<label
					for="my-drawer"
					aria-label="close sidebar"
					class="d-drawer-overlay"
				></label>
				<DaisyUiMenu
					className="bg-base-200 text-base-content min-h-full w-fit "
				>
					<DaisyUiAvatar className="d-avatar-placeholder">
						<div
							class="bg-neutral text-neutral-content w-10 rounded-full"
						></div></DaisyUiAvatar
					>
					<p class="">Mari2020</p>
					<p>Mari2020@gmail.com</p>

					<DaisyUiButton
						className=""
						onClick={() => console.log('Hello')}
						>Change Account</DaisyUiButton
					>

					<div class="">
						<h1 class="">All Pages</h1>

						<div class="leading-5">
							<li><a href="">Pages 1</a></li>
							<li><a href="">Pages 2</a></li>
							<li><a href="">Pages 3</a></li>
						</div>

						<h1 class="">Categories</h1>

						<div class="leading-5">
							<li><a href="">Category 1</a></li>
							<li><a href="">Category 2</a></li>
							<li><a href="">Category 3</a></li>
						</div>

						<h1 class="">Help & Support</h1>

						<div class="">
							<li><a href="">Contact Us</a></li>
							<li><a href="">FAQ</a></li>
						</div>
					</div>
				</DaisyUiMenu>
			</div>
		</div>
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
				onClick={() => goToRoute('/app/notifications')}
			>
				<LucideBell />
			</DaisyUiButton>
		</DaisyUiStatus>
	</DaisyUiNavbarEnd>
</DaisyUiNavbar>
