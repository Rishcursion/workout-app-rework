<script lang="ts">
	import type { ComponentType } from 'svelte';

	let {
		title = '',
		icon,
		body = ''
	}: { title: string; icon: ComponentType; body: string } = $props();
</script>

<div class="rounded-xl bg-white bg-opacity-10 p-6 backdrop-blur-sm">
	<div class="mb-4 text-white">
		<svelte:component this={icon} size={32} />
	</div>
	<h3 class="mb-2 text-xl font-bold text-white">{title}</h3>
	<p class="font-semibold text-white text-opacity-80">{body}</p>
</div>
