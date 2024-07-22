<!-- <script lang="ts">
	import type { IWidgetItem } from '../config/type';

	export let widgetItem: IWidgetItem;
</script>

	<div class="flex-1 bg-amber-300">1</div>
	<div class="">
		<div class="w-80 bg-amber-500">2</div>
		<div class="w-80 bg-amber-700">3</div>
	</div> -->
<script lang="ts">
	import type { IWidgetItem } from '../config/type';
	export let widget: IWidgetItem;
</script>

<div class="bg-background-primary-reversed h-full p-4 md:p-5 lg:p-6">
	<div>
		<a href={widget.ctaLink} target="_self">
			<picture>
				<img
					alt={widget.title}
					class="h-full w-full object-cover object-center"
					loading="lazy"
					src={widget.img}
				/>
			</picture>
		</a>
	</div>
	<div class="font-regular z-10 flex flex-col gap-2 text-left">
		<strong class="heading medium">{widget.title}</strong>
	</div>
	<div class="relative z-10 mt-4">
		<button
			type="button"
			class="btn btn-primary shrink-0 bg-blue-700 px-4 py-2 font-bold text-white hover:bg-blue-900"
			role="link"
			on:click={() => (window.location.href = widget.ctaLink)}
		>
			{widget.ctaLabel}
		</button>
	</div>
</div>
