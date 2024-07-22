<script lang="ts">
	import WidgetItem from './widgetItem.svelte';
	import type { IWidgetItem } from '../config/type';

	export let widgetList: IWidgetItem[];
</script>

<div class="container mx-auto mb-6 flex flex-wrap sm:mb-7 md:mb-8 lg:mb-9">
	<div class="w-full md:w-1/2">
		{#each widgetList as widget (widget.title)}
			{#if widget.main}
				<WidgetItem {widget} />
			{/if}
		{/each}
	</div>
	<div class="flex w-full flex-col justify-between md:w-1/2">
		{#each widgetList as widget (widget.title)}
			{#if !widget.main}
				<WidgetItem {widget} class="mb-3 h-full md:mb-0" />
			{/if}
		{/each}
	</div>
</div>
