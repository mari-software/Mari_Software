<script>
	import LFaqs from '$lib/component/local/index/app/faqs/LFaqs.svelte';
	const dummyData = [
		{
			id: 1,
			question: 'Question 1',
			answer:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. '
		},
		{
			id: 2,
			question: 'Question 2',
			answer:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. '
		},
		{
			id: 3,
			question: 'Question 3',
			answer:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat, officia. '
		}
	];
</script>

<section id="notifications-page" class="my-5 flex flex-col gap-5 p-3">
	<LFaqs {dummyData} />
</section>
