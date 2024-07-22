<script lang="ts">
	import type { IProductMarketing } from '../config/type';
	import MarketingBloc from '../components/marketingBloc.svelte';
	import ProductHighlightItem from './productHighlightItem.svelte';

	export let products: IProductMarketing[];
</script>

<div class="marketing-container flex">
	<MarketingBloc />

	<div class="marketing-product ml-8 flex gap-6 ">
		{#each products as product}
			<ProductHighlightItem {product} />
		{/each}
	</div>
</div>

<style>
	.marketing-product {
		position: relative;
	}
</style>
