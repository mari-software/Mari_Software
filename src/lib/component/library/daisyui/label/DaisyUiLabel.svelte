<script lang="ts">
	let { className, forName, children } = $props<{
		className?: string;
		forName?: string;
		children?: () => void;
	}>();
</script>

<label for={forName} class={className}>
	{@render children()}
</label>
