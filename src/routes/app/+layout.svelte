<script lang="ts">
	import GIndexFooter from '$lib/component/global/index/app/GIndexFooter.svelte';
	import GIndexNavbar from '$lib/component/global/index/app/GIndexNavbar.svelte';

	let { children } = $props();
</script>

<section id="app" class="m-web">
	<section id="navbar">
		<GIndexNavbar />
	</section>
	<main id="main" class="m-main">
		{@render children()}
	</main>
	<section id="footer">
		<GIndexFooter />
	</section>
</section>
