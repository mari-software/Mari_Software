<script>
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
	import DaisyUiInputField from '$lib/component/library/daisyui/inputfield/DaisyUiInputField.svelte';
	import DaisyUiLabel from '$lib/component/library/daisyui/label/DaisyUiLabel.svelte';
	import DaisyUiSelect from '$lib/component/library/daisyui/select/DaisyUiSelect.svelte';
	import DaisyUiTextarea from '$lib/component/library/daisyui/textarea/DaisyUiTextarea.svelte';
	import LucideSearch from '$lib/component/library/lucide/LucideSearch.svelte';
</script>

<section id="contact" class="flex flex-col gap-7">
	<h2 class="m-h2">Do you have a question?</h2>

	<section id="email" class="flex flex-col gap-2">
		<h3 class="m-h3">Enter your email</h3>
		<DaisyUiLabel className="d-input w-full">
			<DaisyUiInputField
				className=""
				inputPlaceholderText="johndoe@example.com"
				inputType="email"
			/>
		</DaisyUiLabel>
	</section>

	<section id="reason" class="flex flex-col gap-2">
		<h3 class="m-h3">Choose your reason</h3>
		<DaisyUiSelect optionHeader="Choose Topic" className="w-full">
			<option>Topic 1</option>
			<option>Topic 2</option>
			<option>Topic 3</option>
		</DaisyUiSelect>
	</section>

	<section id="description" class="flex flex-col gap-2">
		<h3 class="m-h3">Description</h3>
		<DaisyUiTextarea
			className="w-full h-36"
			placeholder="Enter detailed description of your question or issue ..."
		/>
	</section>

	<section id="action">
		<DaisyUiButton
			className="d-btn-primary w-full"
			onClick={() => console.log()}
		>
			Submit
		</DaisyUiButton>
	</section>
</section>
