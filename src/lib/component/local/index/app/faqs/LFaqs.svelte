<script lang="ts">
	import DaisyUiAccordion from '$lib/component/library/daisyui/accordion/DaisyUiAccordion.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
	import DaisyUiInputField from '$lib/component/library/daisyui/inputfield/DaisyUiInputField.svelte';
	import DaisyUiLabel from '$lib/component/library/daisyui/label/DaisyUiLabel.svelte';
	import LucideSearch from '$lib/component/library/lucide/LucideSearch.svelte';

	let { dummyData } = $props<{}>();
</script>

<section id="faqs" class="flex flex-col gap-7">
	<section id="search" class="flex flex-col gap-4">
		<h2 class="m-h2">Frequently Asked Questions</h2>
		<DaisyUiLabel className="d-input w-full">
			<DaisyUiInputField
				className=""
				inputPlaceholderText="Press here to start typing"
				inputType="search"
			/>
			<LucideSearch className="h-[1em] opacity-50" />
		</DaisyUiLabel>
	</section>
	<section id="lists" class="flex flex-col gap-3">
		{#each dummyData as faq}
			<DaisyUiCard>
				<DaisyUiAccordion
					title={faq.question}
					titleClass="m-h3"
					content={faq.answer}
					groupName="faq"
					icon="plus"
				/>
			</DaisyUiCard>
		{/each}
	</section>
</section>
