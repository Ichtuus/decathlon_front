<script lang="ts">
	import type { IPresentation } from '../config/type';
	import PresentationItem from './presentationItem.svelte';

	export let presentations: IPresentation[];
</script>

<div class="flex w-full gap-6">
	{#each presentations as presentation}
		<PresentationItem {presentation} />
	{/each}
</div>
