<script>
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import LCategorySearchFilter from '$lib/component/local/index/app/main/categories/category/LCategorySearchFilter.svelte';
	import LCategoryProductList from '$lib/component/local/index/app/main/categories/LCategoryProductList.svelte';

	const dummyData = [
		{
			id: 1,
			icon: MariLogoSvg,
			name: 'Product Name',
			description: 'This is description'
		},
		{
			id: 2,
			icon: MariLogoSvg,
			name: 'Product Name',
			description: 'This is description'
		},
		{
			id: 3,
			icon: MariLogoSvg,
			name: 'Product Name',
			description: 'This is description'
		},
		{
			id: 4,
			icon: MariLogoSvg,
			name: 'Product Name',
			description: 'This is description'
		}
	];
</script>

<section id="product-page" class="my-5 flex flex-col gap-10 p-3">
	<section id="search-filter">
		<LCategorySearchFilter />
	</section>
	<section id="">
		<LCategoryProductList {dummyData} />
	</section>
</section>
