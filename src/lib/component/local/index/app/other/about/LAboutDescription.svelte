<script>
	import DaisyUiButton from '$lib/component/library/daisyui/button/DaisyUiButton.svelte';
</script>

<section id="description" class="flex flex-col gap-2">
	<p>This is the description about MARI</p>
	<p>
		Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta
		deserunt natus iste obcaecati odit dolor nobis quidem ab adipisci
		id consequatur, nisi ea beatae voluptatum cumque reprehenderit
		inventore maxime eum.
	</p>
	<DaisyUiButton
		className="d-btn-primary w-auto self-center my-3"
		onClick={() => console.log()}
	>
		View More
	</DaisyUiButton>
</section>
