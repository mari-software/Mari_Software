<script>
	import DaisyUiInputField from '$lib/component/library/daisyui/inputfield/DaisyUiInputField.svelte';
	import DaisyUiLabel from '$lib/component/library/daisyui/label/DaisyUiLabel.svelte';
	import LucideSearch from '$lib/component/library/lucide/LucideSearch.svelte';
</script>

<section id="search-filter" class="flex flex-col items-center gap-4">
	<h1 class="m-h3">What would you like to search?</h1>
	<DaisyUiLabel className="d-input w-full">
		<DaisyUiInputField
			className=""
			inputPlaceholderText="Press here to start typing"
			inputType="search"
		/>
		<LucideSearch className="h-[1em] opacity-50" />
	</DaisyUiLabel>
</section>
