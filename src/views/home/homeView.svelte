<script lang="ts">
	import WidgetContainer from '../../features/widgets/views/widgetContainer.svelte';
	import PubContainer from '../../features/pub/views/pubContainer.svelte';
	import CategoriesContainer from '../../features/categories/views/categoriesContainer.svelte';
	import PresentationContainer from '../../features/presentations/views/presentationContainer.svelte';
	import ProductHighlightContainer from '../../features/product-highlight/views/productHighlightContainer.svelte';
</script>

<div class="flex flex-wrap gap-24">
	<WidgetContainer />

	<PubContainer />

	<CategoriesContainer />

	<PresentationContainer />

	<ProductHighlightContainer />
</div>
