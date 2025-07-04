<script lang="ts">
	import { goto } from '$app/navigation';
	import Example from '$lib/component/local/app/Example.svelte';
	import { onMount } from 'svelte';

	onMount(() => {
		goto('/app')
	});
	
</script>





