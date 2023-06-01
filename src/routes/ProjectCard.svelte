<script>
	import TechBadge from './TechBadge.svelte';
	export let project;
	let { title, image, description, technologies } = project;
	image = image.href || image.local;
</script>

<div class="max-w-sm bg-white  rounded-lg shadow lg:max-w-full">
	<a href="#">
		<img class="rounded-t-lg w-full h-44 object-cover" src={image} alt="" />
	</a>
	<div class="p-5">
		<a href="#" class="mb-2 block">
			<h5 class="text-2xl font-bold tracking-tight text-gray-900 ">
				{title}
			</h5>
		</a>
		<p class=" font-normal text-gray-700">
			{description.slice(0, 100) + '...'}
		</p>
		<hr class="my-3" />

		<div class="w-full mb-3">
			<h4 class="text-gray-500 text-sm">Built with:</h4>
			{#each technologies as tech}
				<TechBadge text={tech} />
			{/each}
		</div>

		<button
			class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-indigo-600 rounded-lg hover:bg-indigo-800 focus:ring-4 focus:outline-none focus:ring-blue-300"
		>
			<a>Read more</a>
			<svg
				aria-hidden="true"
				class="w-4 h-4 ml-2 -mr-1"
				fill="currentColor"
				viewBox="0 0 20 20"
				xmlns="http://www.w3.org/2000/svg"
				><path
					fill-rule="evenodd"
					d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
					clip-rule="evenodd"
				/></svg
			>
		</button>
	</div>
</div>
