<script lang="ts">
	let { className, forText, children } = $props<{
		className?: string;
		forText?: string;

		children?: () => void;
	}>();
</script>

<label for={forText} class={className}>
	{@render children()}
</label>
