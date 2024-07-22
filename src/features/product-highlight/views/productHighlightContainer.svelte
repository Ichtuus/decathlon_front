<script lang="ts">
	import type { IProductMarketing } from '../config/type';
	import ProductHighlightList from './ProductHighlightList.svelte';

	const products: IProductMarketing[] = [
		{
			img: 'https://contents.mediadecathlon.com/p2061338/k$26717eabad61aa86ed85a3ec1d2a87a5/sq/8665089.jpg?format=auto&f=160x160',
			availabilityDate:
				'À partir du 10/07/2024 et avant le 24/07/2024 dans la limite des stocks disponibles',
			desc: 'Boardshort Court Quiksilver Homme Orange Claire',
			discountAmount: '-11€',
			discountPrice: '19€',
			price: '30€',
			shipText: 'Livraison en 48h',
			title: 'QUIKSILVER'
		},
		{
			img: 'https://contents.mediadecathlon.com/p2514096/k$d7832fb73b957a8266b204ca1693b1c9/sq/8832822.jpg?format=auto&f=160x160',
			availabilityDate:
				'À partir du 10/07/2024 et avant le 24/07/2024 dans la limite des stocks disponibles',
			desc: 'LEGGING TECHFIT DE FITNESS CARDIO ADIDAS FEMME NOIR',
			discountAmount: '-25€',
			discountPrice: '25€',
			price: '50€',
			shipText: 'Livraison en 48h',
			title: 'Adidas'
		},
		{
			img: 'https://contents.mediadecathlon.com/p2611525/k$737fd8c52b8a7bb2b48fa7f18e85afa8/sq/8881240.jpg?format=auto&f=160x160',
			availabilityDate:
				'À partir du 10/07/2024 et avant le 24/07/2024 dans la limite des stocks disponibles',
			desc: 'CHAUSSURE DE RUNNING HOMME ASICS - GEL-PULSE 15 H NOIR JAUNE',
			discountAmount: '-44€',
			discountPrice: '66€',
			price: '110€',
			shipText: 'Livraison en 48h',
			title: 'Asics'
		}
	];
</script>

<ProductHighlightList {products} />
