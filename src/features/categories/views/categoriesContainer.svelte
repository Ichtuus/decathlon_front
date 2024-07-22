<script lang="ts">
	import CategoriesList from './categoriesList.svelte';
	import type { ICategories } from '../config/type';

	const categories: ICategories[] = [
		{ label: 'Femme', highlight: false },
		{ label: 'Homme', highlight: false },
		{ label: 'Enfant', highlight: false },
		{ label: 'Equipement', highlight: false },
		{ label: 'Réparation', highlight: false },
		{ label: 'Soldes & Bons plans', highlight: true }
	];
</script>

<CategoriesList {categories} />
