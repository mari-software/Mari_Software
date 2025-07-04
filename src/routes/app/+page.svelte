<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import LAppArticles from '$lib/component/local/index/app/LAppArticles.svelte';
	import LAppHeroBanner from '$lib/component/local/index/app/LAppHeroBanner.svelte';
	import LAppHighlight from '$lib/component/local/index/app/LAppHighlight.svelte';
	import LAppProductLine from '$lib/component/local/index/app/LAppProductLine.svelte';
	import LAppSearchFilter from '$lib/component/local/index/app/LAppSearchFilter.svelte';

	let productLines = $state([
		[
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
		],
		[
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
		],
		[
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
		]
	]);

	const articleLines = $state([
		{
			id: 1,
			title: 'Article - 1',
			description: 'This is description'
		},
		{
			id: 2,
			title: 'Article - 2',
			description: 'This is description'
		},
		{
			id: 3,
			title: 'Article - 3',
			description: 'This is description'
		},
		{
			id: 4,
			title: 'Article - 4',
			description: 'This is description'
		}
	]);
</script>

<section id="app-page" class="mt-5 flex flex-col gap-5 p-3">
	<section id="hero">
		<LAppHeroBanner />
	</section>
	<section id="highlight">
		<LAppHighlight />
	</section>
	<section id="search-filter" class="mt-2">
		<LAppSearchFilter />
	</section>
	<section id="product-lines" class="flex flex-col gap-7">
		{#each productLines as productLine, i}
			<LAppProductLine {productLine} {i} />
		{/each}
	</section>
	<section id="articles">
		<LAppArticles {articleLines} />
	</section>
</section>
