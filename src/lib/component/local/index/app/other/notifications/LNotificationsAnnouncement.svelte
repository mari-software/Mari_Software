<script lang="ts">
	import DaisyUiCardBody from '$lib/component/library/daisyui/card/body/DaisyUiCardBody.svelte';
	import DaisyUiCardBodyTitle from '$lib/component/library/daisyui/card/body/title/DaisyUiCardBodyTitle.svelte';
	import DaisyUiCard from '$lib/component/library/daisyui/card/DaisyUiCard.svelte';
	import DaisyUiStatus from '$lib/component/library/daisyui/status/DaisyUiStatus.svelte';

	let { notification } = $props<{}>();
</script>

<section id="announcement" class="flex flex-col gap-4">
	{#each notification as n}
		<DaisyUiCard className="bg-base-300 shadow-lg">
			<DaisyUiCardBody>
				<DaisyUiCardBodyTitle>
					{#if n.important}
						{#if n.important == 0}
							<DaisyUiStatus className="d-status-neutral " />
							<h3>{n.title}</h3>
						{:else if n.important == 1}
							<DaisyUiStatus className="d-status-primary" />
							<h3>{n.title}</h3>
						{:else if n.important == 2}
							<DaisyUiStatus className="d-status-error" />
							<h3>{n.title}</h3>
						{/if}
					{:else}
						<DaisyUiStatus className="d-status-neutral" />
						<h3>{n.title}</h3>
					{/if}
				</DaisyUiCardBodyTitle>
				<p>{n.description}</p>
			</DaisyUiCardBody>
		</DaisyUiCard>
	{/each}
</section>
