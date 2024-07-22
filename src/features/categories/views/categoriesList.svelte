<script lang="ts">
	import CategoriesItem from './categoriesItem.svelte';
	import type { ICategories } from '../config/type';

	export let categories: ICategories[];
</script>

<div class="flex w-full gap-6">
	{#each categories as categorie}
		<CategoriesItem {categorie} />
	{/each}
</div>
