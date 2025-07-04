<script lang="ts">
	let { effect, className, children } = $props<{
		effect?: 'ping' | 'bounce';
		className?: string;
		children?: () => void;
	}>();
</script>

<div class="relative inline-block">
	<div class="relative">
		{@render children()}
	</div>

	<!-- Animated status badge -->
	<div
		class="d-status absolute top-0 right-0 {className} animate-{effect}"
	></div>

	{#if effect === 'ping'}
		<!-- Static status below the animated one for ping effect -->
		<div class="d-status absolute top-0 right-0 {className}"></div>
	{/if}
</div>
