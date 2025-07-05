<script lang="ts">
	import LNotificationsAnnouncement from './LNotificationsAnnouncement.svelte';
	import LNotificationsUpdates from './LNotificationsUpdates.svelte';

	let { notification } = $props<{}>();
</script>

<section id="notifications" class="flex flex-col gap-5">
	<section id="header">
		<h2 class="m-h2">Notifications</h2>
	</section>
	<section id="updates" class="flex flex-col gap-3">
		<h2 class="m-h2">Updates</h2>
		<LNotificationsUpdates {notification} />
	</section>
	<section id="announcement" class="flex flex-col gap-3">
		<h2 class="m-h2">Announcement</h2>
		<LNotificationsAnnouncement {notification} />
	</section>
</section>
