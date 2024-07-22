<script lang="ts">
	import type { IPresentation } from '../config/type';

	export let presentation: IPresentation;
</script>

<div class="inline-block flex-1 p-6 font-bold">
	<img src={presentation.img} alt="" class="pb-2" />
	{presentation.title}
</div>
