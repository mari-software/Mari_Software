<script>
	import LNotificationsWrapper from '$lib/component/local/index/app/other/notifications/LNotificationsWrapper.svelte';

	const notification = [
		{
			id: 1,
			title: 'Notification Title',
			description: 'Notification Description',
			date: new Date(),
			important: 0
		},
		{
			id: 2,
			title: 'Notification Title',
			description: 'Notification Description',
			date: new Date(),
			important: 1
		},
		{
			id: 3,
			title: 'Notification Title',
			description: 'Notification Description',
			date: new Date(),
			important: 2
		}
	];
</script>

<section id="notifications-page" class="my-5 flex flex-col gap-5 p-3">
	<LNotificationsWrapper {notification} />
</section>
