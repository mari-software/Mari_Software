<script lang="ts">
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import LProductAccess from '$lib/component/local/index/app/main/products/product/LProductAccess.svelte';
	import LProductHeader from '$lib/component/local/index/app/main/products/product/LProductHeader.svelte';

	// let { data } = $props<{}>();

	const product = {
		id: 1,
		icon: MariLogoSvg,
		name: 'Mari Software',
		groupName: 'software.mari',
		description:
			'This is a short description of the product. It will not go more than 2 sentences.',
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
		]
	};
</script>

<section id="product-page" class="my-5 flex flex-col gap-5 p-3">
	<section id="header">
		<LProductHeader {product} />
	</section>
	<section id="stats">
		<LProductAccess {product} />
	</section>
</section>
