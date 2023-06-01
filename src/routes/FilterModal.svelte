<script>
	import TechBadge from './TechBadge.svelte';
	export let filterTechnologies;
	export let technologies;
	let modalOpen = false;
</script>

<!-- Modal toggle -->

<button
	class="block text-white focus:text-[#151518] focus:bg-white focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-3 py-1.5 text-center border"
	type="button"
	on:click={() => (modalOpen = !modalOpen)}
>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		fill="none"
		viewBox="0 0 24 24"
		stroke-width="1.5"
		stroke="currentColor"
		class="w-6 h-6 lg:h-8 lg:w-8"
	>
		<path
			stroke-linecap="round"
			stroke-linejoin="round"
			d="M10.5 6h9.75M10.5 6a1.5 1.5 0 11-3 0m3 0a1.5 1.5 0 10-3 0M3.75 6H7.5m3 12h9.75m-9.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-3.75 0H7.5m9-6h3.75m-3.75 0a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m-9.75 0h9.75"
		/>
	</svg>
</button>

<!-- Main modal -->
<div
	id="defaultModal"
	tabindex="-1"
	class={'fixed top-20 left-0 lg:hidden right-0 z-50 w-full  overflow-x-hidden overflow-y-auto p-4  md:inset-0 h-[calc(100%-7rem)] max-h-full' +
		(modalOpen ? '' : ' hidden')}
>
	<div class="relative w-full max-w-2xl max-h-full">
		<!-- Modal content -->
		<div class="relative bg-white rounded-lg shadow dark:bg-gray-700  ">
			<!-- Modal header -->
			<div class="flex items-start justify-between p-4 border-b rounded-t dark:border-gray-600">
				<h3 class="text-xl font-semibold text-gray-900 dark:text-white">Filter by project</h3>
				<button
					type="button"
					class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm p-1.5 ml-auto inline-flex items-center "
					on:click={() => (modalOpen = !modalOpen)}
				>
					<svg
						aria-hidden="true"
						class="w-5 h-5"
						fill="currentColor"
						viewBox="0 0 20 20"
						xmlns="http://www.w3.org/2000/svg"
						><path
							fill-rule="evenodd"
							d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
							clip-rule="evenodd"
						/></svg
					>
					<span class="sr-only">Close modal</span>
				</button>
			</div>
			<div class="grid grid-cols-2 w-full h-full gap-3 py-6 px-4 ">
				{#each technologies as technology}
					<button
						class={'text-lg font-medium mr-2 px-2.5 py-0.5 rounded w-full py-8 border ' +
							(filterTechnologies.includes(technology)
								? 'bg-gray-400 text-white'
								: 'text-gray-400 bg-white')}
						on:click={() => {
							if (!filterTechnologies.includes(technology)) {
								filterTechnologies = [...filterTechnologies, technology];
							} else {
								filterTechnologies = filterTechnologies.filter((t) => t !== technology);
							}
						}}
					>
						{technology}
					</button>
				{/each}
			</div>
		</div>
	</div>
</div>

<div
	id="defaultModal"
	tabindex="-1"
	class={'fixed pt-16 pl-[35%] w-[100%] hidden lg:block z-50 overflow-x-hidden overflow-y-auto p-4  md:inset-0 h-[calc(100%-7rem)] max-h-full' +
		(modalOpen ? '' : ' lg:hidden')}
>
	<div class="relative w-full max-w-2xl max-h-full">
		<!-- Modal content -->
		<div class="relative bg-white rounded-lg shadow dark:bg-gray-700  ">
			<!-- Modal header -->
			<div class="flex items-start justify-between p-4 border-b rounded-t dark:border-gray-600">
				<h3 class="text-xl font-semibold text-gray-900 dark:text-white">Filter by project</h3>
				<button
					type="button"
					class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm p-1.5 ml-auto inline-flex items-center "
					on:click={() => (modalOpen = !modalOpen)}
				>
					<svg
						aria-hidden="true"
						class="w-5 h-5"
						fill="currentColor"
						viewBox="0 0 20 20"
						xmlns="http://www.w3.org/2000/svg"
						><path
							fill-rule="evenodd"
							d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
							clip-rule="evenodd"
						/></svg
					>
					<span class="sr-only">Close modal</span>
				</button>
			</div>
			<div class="grid grid-cols-2 w-full h-full gap-3 py-6 px-4 ">
				{#each technologies as technology}
					<button
						class={'text-lg font-medium mr-2 px-2.5 py-0.5 rounded w-full py-8 border ' +
							(filterTechnologies.includes(technology)
								? 'bg-gray-400 text-white'
								: 'text-gray-400 bg-white')}
						on:click={() => {
							if (!filterTechnologies.includes(technology)) {
								filterTechnologies = [...filterTechnologies, technology];
							} else {
								filterTechnologies = filterTechnologies.filter((t) => t !== technology);
							}
						}}
					>
						{technology}
					</button>
				{/each}
			</div>
		</div>
	</div>
</div>
