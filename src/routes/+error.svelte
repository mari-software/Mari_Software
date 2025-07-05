<script lang="ts">
	import GIndexFooter from '$lib/component/global/index/app/GIndexFooter.svelte';
	import GIndexNavbar from '$lib/component/global/index/app/GIndexNavbar.svelte';
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import {
		goBackRoute,
		goToRoute
	} from '$lib/util/sveltekit/router.sveltekit.util';
</script>

<section id="app" class="m-app">
	<section id="navbar">
		<GIndexNavbar />
	</section>
	<main id="main" class="m-main">
		<section
			id="not-found"
			class="m-auto flex flex-col items-center justify-center gap-5 py-32"
		>
			<div>
				<h1 class="m-h1 text-error">404 Page Not Found</h1>
				<p class="m-h4 opacity-50">MARI.SOFTWARE</p>
			</div>
			<div class="flex w-full justify-end gap-3">
				<DaisyUiButton onClick={goBackRoute}>Go Back</DaisyUiButton>
				<DaisyUiButton
					className="d-btn-primary"
					onClick={() => goToRoute('/')}>Home</DaisyUiButton
				>
			</div>
		</section>
	</main>
	<section id="footer">
		<GIndexFooter />
	</section>
</section>
