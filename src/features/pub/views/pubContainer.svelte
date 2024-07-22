<script lang="ts">
	import type { IPubData } from '../config/type';

	const olympicsDate = '2024-07-26';

	function getDaysUntil(targetDate: string): number {
		const today = new Date();
		const eventDate = new Date(targetDate);
		const timeDiff = eventDate.getTime() - today.getTime();
		return Math.ceil(timeDiff / (1000 * 3600 * 24));
	}

	const pubData: IPubData = {
		bgImg: '',
		img: 'https://www.decathlon.media/dossier-presse/2021/jo-paris-2024/landing/v0.4/--livrables--/img/decathlon-jo-paris-2024_twitter.jpg',
		label: `j-${getDaysUntil(olympicsDate)} avant les Jeux Olympiques de Paris 2024`,
		ctaLabel: 'Découvrez notre collection officielle',
		ctaLink: ''
	};
</script>

<div class="grid grid-cols-3 items-center gap-5 rounded-full" style="background-color: #07178a;">
	<div
		style="background-image: url('https://contents.mediadecathlon.com/s1083368/k$8a3e3aa5b3b0087c42e960a1c0df61f2/JO%20motif%20gauche.png'); background-size: 100% auto;"
		class="h-20 w-72 justify-self-start rounded-full"
	></div>
	<div class="justify-self-center text-white">{pubData.label}</div>
	<div
		class="flex h-20 w-72 items-center justify-self-start justify-self-end rounded-full"
		style="background-image: url('https://contents.mediadecathlon.com/s1083370/k$21a8443e4af5b326795b58aa18f41019/JO%20motif%20droit.png'); background-size: 100% auto;"
	>
		<button
			type="button"
			class=" rounded-full bg-neutral-50 px-5 py-2.5 text-sm font-medium text-blue-700 hover:bg-transparent focus:outline-none focus:ring-4 focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
			>{pubData.ctaLabel}</button
		>
	</div>
</div>
