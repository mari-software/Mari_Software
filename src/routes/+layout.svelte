<script lang="ts">
	import GIndexFooter from '$lib/component/global/index/GIndexFooter.svelte';
	import GIndexNavbar from '$lib/component/global/index/GIndexNavbar.svelte';
	import '../app.css';

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
