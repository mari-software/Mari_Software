<script>
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import LAboutCollaboratingUnits from '$lib/component/local/index/app/other/about/LAboutCollaboratingUnits.svelte';
	import LAboutDescription from '$lib/component/local/index/app/other/about/LAboutDescription.svelte';
	import LAboutGoals from '$lib/component/local/index/app/other/about/LAboutGoals.svelte';
	import LAboutHeader from '$lib/component/local/index/app/other/about/LAboutHeader.svelte';
	import LAboutMission from '$lib/component/local/index/app/other/about/LAboutMission.svelte';
	import LAboutSponsors from '$lib/component/local/index/app/other/about/LAboutSponsors.svelte';
	import LAboutVision from '$lib/component/local/index/app/other/about/LAboutVision.svelte';

	const dummyData = [
		{
			id: 1,
			name: 'Product Name',
			icon: MariLogoSvg
		},
		{
			id: 1,
			name: 'Product Name',
			icon: MariLogoSvg
		},
		{
			id: 1,
			name: 'Product Name',
			icon: MariLogoSvg
		},
		{
			id: 1,
			name: 'Product Name',
			icon: MariLogoSvg
		}
	];
</script>

<section id="about-page" class="my-5 flex flex-col gap-5 p-3">
	<section id="header">
		<LAboutHeader />
	</section>
	<section id="description">
		<LAboutDescription />
	</section>
	<section id="vision">
		<LAboutVision />
	</section>
	<section id="mission">
		<LAboutMission />
	</section>
	<section id="goals">
		<LAboutGoals />
	</section>
	<section id="collaborating-units">
		<LAboutCollaboratingUnits {dummyData} />
	</section>
	<section id="sponsors">
		<LAboutSponsors {dummyData} />
	</section>
</section>
