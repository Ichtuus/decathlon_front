<script lang="ts">
	import type { IWidgetItem } from '../config/type';
	import WidgetList from './widgetList.svelte';

	const widgetList: IWidgetItem[] = [
		{
			title: 'Exclu Web',
			img: 'https://contents.mediadecathlon.com/s1107914/auto/.jpg?format=auto&f=undefinedx0',
			main: true,
			ctaLabel: 'Voir la sélection',
			ctaLink: '#'
		},
		{
			title: 'Quechua glacière de camping',
			img: 'https://contents.mediadecathlon.com/s1119742/auto/.jpg?format=auto&f=undefinedx0',
			main: false,
			ctaLabel: "J'en profite",
			ctaLink: '#'
		},
		{
			title: 'Qui aime bien bichonne bien',
			img: 'https://contents.mediadecathlon.com/s1117533/auto/.jpg?format=auto&f=undefinedx0',
			main: false,
			ctaLabel: 'Voir toutes nos pièce détachées',
			ctaLink: '#'
		}
	];
</script>

<div class="container mx-auto">
	<WidgetList {widgetList} />
</div>
