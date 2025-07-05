<script lang="ts">
	let {
		className,
		inputPlaceholderText,
		inputType,
		inputPattern,
		inputTitle,
		minLength,
		maxlength,
		nameText
	} = $props<{
		className?: string;
		inputPlaceholderText?: string;
		inputType?: string;
		inputPattern?: string;
		inputTitle?: string;
		minLength?: number;
		maxlength?: number;
		nameText?: string;
	}>();
</script>

<input
	class="d-input {className}"
	type={inputType}
	required
	placeholder={inputPlaceholderText}
	pattern={inputPattern}
	minlength={minLength ?? 1}
	maxlength={maxlength ?? 50}
	title={inputTitle}
	name={nameText}
/>
