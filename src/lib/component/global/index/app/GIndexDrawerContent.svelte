<script>
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiAvatar from '$lib/component/library/daisyui/avatar/DaisyUiAvatar.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
</script>

<section id="drawer-content" class="flex flex-col gap-3 px-5 py-3">
	<!-- Account Info -->
	<section id="account" class="flex justify-between">
		<DaisyUiAvatar>
			<MariLogoSvg className="size-14" />
		</DaisyUiAvatar>
		<section id="account-info">
			<h3 class="m-h3">Mari2025</h3>
			<p>mari2025@exampl.com</p>
		</section>
	</section>

	<!-- Account Action Button -->
	<section id="account-action">
		<DaisyUiButton
			className="d-btn-neutral d-btn-wide"
			onClick={() => console.log()}
		>
			Change Account
		</DaisyUiButton>
	</section>

	<!-- Pages -->
	<section id="all-pages" class="mt-5 flex flex-col gap-5">
		<h3 class="m-h3">All Pages</h3>
		<section id="pages-buttons" class="flex flex-col gap-2">
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Pages 1
			</DaisyUiButton>
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Pages 2
			</DaisyUiButton>
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Pages 3
			</DaisyUiButton>
		</section>
	</section>

	<!-- Category -->
	<section id="all-categories" class="mt-5 flex flex-col gap-5">
		<h3 class="m-h3">Categories</h3>
		<section id="pages-buttons" class="flex flex-col gap-2">
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Category 1
			</DaisyUiButton>
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Category 2
			</DaisyUiButton>
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Category 3
			</DaisyUiButton>
		</section>
	</section>

	<!-- Help & Support  -->
	<section id="help-and-support" class="mt-5 flex flex-col gap-5">
		<h3 class="m-h3">Help & Support</h3>
		<section id="pages-buttons" class="flex flex-col gap-2">
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				Contact Us
			</DaisyUiButton>
			<DaisyUiButton
				className="d-btn-ghost justify-start"
				onClick={() => console.log('Hello')}
			>
				FAQ
			</DaisyUiButton>
		</section>
	</section>
</section>
