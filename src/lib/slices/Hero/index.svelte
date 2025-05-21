<script lang="ts">
	import type { Content } from '@prismicio/client';

	export let slice: Content.HeroSlice;
</script>

<section
	data-slice-type={slice.slice_type}
	data-slice-variation={slice.variation}
	class="px-4 md:px-6"
>
	<div class="grid min-h-[65vh] grid-cols-1 items-center md:grid-cols-2">
		<div
			class="relative z-10 row-span-1 row-start-1 -my-10 aspect-[1/1.3] overflow-hidden md:col-span-1 md:col-start-2 md:mt-0"
		>
			Shape Scene
		</div>
		<div class="mx-auto w-full max-w-7xl">
			<h1
				class="mb-2 md:mb-8 text-[clamp(3rem,20vmin,13rem)] font-extrabold leading-none tracking-tighter text-nowrap"
			>
				<span class="block text-violet-300">
					{slice.primary.first_name}
				</span>
				<span class="block text-violet-500 -mt-[.2em]">
					{slice.primary.last_name}
				</span>
			</h1>
			<span
				class="block bg-gradient-to-tr from-sky-500 via-sky-100 to-sky-500 bg-clip-text text-transparent text-2xl font-bold uppercase tracking-[.2em] md:text-4xl"
			>
				{slice.primary.tag_line}
			</span>
		</div>
	</div>
</section>
