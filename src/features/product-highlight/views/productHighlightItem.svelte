<script lang="ts">
	import type { IProductMarketing } from '../config/type';

	export let product: IProductMarketing;
</script>

<div class="w-48 border border-slate-50">
	<img class="mb-16" src={product.img} alt="" />
	<span class="sold bg-red-600 pl-2 pr-2 text-white">Soldes</span>
	<div class="mb-4 gap-3">
		<span class="mr-2 bg-red-600 pb-2 pl-3 pr-3 pt-2 text-white">{product.discountPrice}</span>
		<span class="mr-2 text-xs line-through">{product.price}</span>
		<span class="font-bold text-red-600">{product.discountAmount}</span>
	</div>

	<p class="text-sm">
		{product.availabilityDate}
	</p>

	<h3 class="text-2xl font-bold uppercase">{product.title}</h3>

	<p class="uppercase">{product.desc}</p>

	<p class="mt-6 text-green-700">{product.shipText}</p>
</div>

<style lang="scss">
	.sold {
		position: absolute;
		top: 1%;
		transform: translate(-50%, -50%);
		-ms-transform: translate(-50%, -50%);
	}
</style>
