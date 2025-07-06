<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import LProductAccess from '$lib/component/local/index/app/main/products/product/LProductAccess.svelte';
	import LProductDetail from '$lib/component/local/index/app/main/products/product/LProductDetail.svelte';
	import LProductHeader from '$lib/component/local/index/app/main/products/product/LProductHeader.svelte';
	import LProductHighlight from '$lib/component/local/index/app/main/products/product/LProductHighlight.svelte';
	import LProductSameCreator from '$lib/component/local/index/app/main/products/product/LProductSameCreator.svelte';
	import LProductSimilarProduct from '$lib/component/local/index/app/main/products/product/LProductSimilarProduct.svelte';

	// let { data } = $props<{}>();

	const product = {
		id: 1,
		icon: MariLogoSvg,
		name: 'Mari Software',
		author: 'mari.software',
		groupName: 'software.mari',
		description:
			'This is a short description of the product. It will not go more than 2 sentences.',
		detailDescription: `
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Deleniti saepe quia magnam ipsa fugiat. Ducimus esse vel ut, temporibus ab perferendis suscipit praesentium sequi excepturi qui id quod! Commodi, ea.
Lorem ipsum, dolor sit amet consectetur adipisicing elit. Deleniti saepe quia magnam ipsa fugiat. Ducimus esse vel ut, temporibus ab perferendis suscipit praesentium sequi excepturi qui id quod! Commodi, ea.
		`,
		category: ['Tag-1', 'Tag-2', 'Tag-3'],
		star: '4.5',
		fileSize: '50',
		download: '50',
		accessLink: [
			{
				name: 'Website',
				link: 'https://google.com'
			},
			{
				name: 'Desktop',
				platforms: [
					{ name: 'Window', link: 'https://google.com' },
					{ name: 'MacOS', link: 'https://google.com' },
					{ name: 'Linux', link: 'https://google.com' }
				]
			},
			{
				name: 'Mobile',
				platforms: [
					{ name: 'Android', link: 'https://' },
					{ name: 'IOS', link: 'https://' }
				]
			},
			{
				name: 'File',
				link: 'https://google.com'
			},
			{
				name: 'Source Code',
				link: 'https://google.com'
			}
		],
		similarProduct: [
			{
				id: 2,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 3,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 4,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 5,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			}
		],
		productBySameCreator: [
			{
				id: 2,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 3,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 4,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			},
			{
				id: 5,
				icon: MariLogoSvg,
				name: 'Another App',
				description: 'This is  description'
			}
		]
	};
</script>

<section id="product-page" class="my-5 flex flex-col gap-10 p-3">
	<section id="header">
		<LProductHeader {product} />
	</section>
	<section id="stats">
		<LProductAccess {product} />
	</section>
	<section id="highlight">
		<LProductHighlight {product} />
	</section>
	<section id="detail">
		<LProductDetail {product} />
	</section>
	<section id="similar-product">
		<LProductSimilarProduct {product} />
	</section>
	<section id="same-creator-product">
		<LProductSameCreator {product} />
	</section>
</section>
