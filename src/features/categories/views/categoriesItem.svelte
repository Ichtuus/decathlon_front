<script lang="ts">
	import type { ICategories } from '../config/type';

	export let categorie: ICategories;
</script>

<div
	class:text-red-700={categorie.highlight}
	class:text-gray-700={!categorie.highlight}
	class="inline-block flex-1 bg-slate-50 p-6 text-center align-middle font-bold"
>
	{categorie.label}
</div>
