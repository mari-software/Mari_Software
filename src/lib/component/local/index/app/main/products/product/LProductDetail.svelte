<script lang="ts">
	let { product } = $props<{}>();
</script>

<section id="detail" class="flex flex-col gap-5">
	<h3 class="m-h3">
		About {product.name}
	</h3>

	<p>
		{product.detailDescription}
	</p>
</section>
