<script lang="ts">
	import type { IPresentation } from '../config/type';
	import PresentationList from './presentationList.svelte';

	const presentations: IPresentation[] = [
		{
			title: "L'été au camping",
			img: 'https://contents.mediadecathlon.com/s1119747/k$24dedc238d6257c1ef52efebe876bfe6/defaut.jpg?format=auto/lete-au-camping.jpg?format=auto&f=900x0'
		},
		{
			title: "L'été à la plage",
			img: 'https://contents.mediadecathlon.com/s1098815/k$f6f50c26e949137b88172de1e68007bd/defaut.jpg?format=auto/lete-a-la-plage.jpg?format=auto&f=900x0'
		},
		{
			title: "L'été à la montagne",
			img: 'https://contents.mediadecathlon.com/s1098814/k$dae9601e9261308eed3f6f190daaef76/defaut.jpg?format=auto/lete-a-la-montagne.jpg?format=auto&f=900x0'
		},
		{
			title: 'Soldes & Bons plans',
			img: 'https://contents.mediadecathlon.com/s1116325/k$e0eec5e4f8bff416fb6a38741baf04ec/defaut.jpg?format=auto/soldes-and-bons-plans.jpg?format=auto&f=900x0'
		},
		{
			title: 'La sélection festival',
			img: 'https://contents.mediadecathlon.com/s1116669/k$9063ecab0ad3b3b384300955e25d05a1/defaut.jpg?format=auto/la-selection-festival.jpg?format=auto&f=900x0'
		},
		{
			title: "L'été à moins de 10€",
			img: 'https://contents.mediadecathlon.com/s1092950/k$fec445e3995ab7193fe05d994f2e9be2/selection%201.jpg?format=auto/lete-a-moins-de-10.jpg?format=auto&f=900x0'
		}
	];
</script>

<PresentationList {presentations} />
