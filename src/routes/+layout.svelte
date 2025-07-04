<script lang="ts">
	import Footer from '$lib/component/global/Footer.svelte';
	import Navbar from '$lib/component/global/Navbar.svelte';

	
	import '../app.css';

	let { children } = $props();
</script>

{@render children()}

<Navbar />
<Footer />





