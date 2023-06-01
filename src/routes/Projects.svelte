<script>
	import FilterModal from './FilterModal.svelte';
	import ProjectCard from './ProjectCard.svelte';
	import TechBadge from './TechBadge.svelte';
	let searchTerm = '';
	$: filteredProjects = projectData.filter((project) => {
		return (
			(project.title.toLowerCase().includes(searchTerm.toLowerCase()) || searchTerm == '') &&
			(filterTechnologies.some((item) => project.technologies.includes(item)) ||
				filterTechnologies.length == 0)
		);
	});

	const projectData = [
		{
			id: 1,
			title: '3D Checkers',
			description:
				'A 3d version of the checkers game made as part of the Masters in Software Engineering. The game was',
			technologies: ['JavaScript', 'HTML', 'CSS', 'WebGL', 'WebCGF'],
			image: {
				href: 'https://raw.githubusercontent.com/luis-viegas/3D-checkers/main/game/screenshots/SGI3_T6_G10_1.png',
				local: ''
			},
			href: 'https://github.com/luis-viegas/3D-checkers'
		},
		{
			id: 2,
			title: 'Decentralized-Twitter',
			description:
				'A decentralized version of twitter, the back-end (for each node) is made in Python',
			technologies: ['JavaScript', 'HTML', 'CSS', 'Python', 'React'],
			image: {
				href: 'https://sm.ign.com/t/ign_pt/screenshot/default/twitter_15fz.1280.jpg',
				local: ''
			},
			href: 'https://github.com/luis-viegas/Decentralized-Twitter'
		},
		{
			id: 3,
			title: 'Gig Arcade',
			description:
				'A system that makes available and tests the games developed by the students of the Faculty of Engineering of the University of Porto.',
			technologies: ['JavaScript', 'HTML', 'CSS', 'NodeJS', 'ElectronJS'],
			image: { href: '', local: 'gig_logo.png' },
			href: 'https://github.com/luis-viegas/GiG-Arcade'
		},
		{
			id: 4,
			title: 'Proteingram',
			description:
				'ProteinGram is a social network dedicated to people who work out, whether at home',
			technologies: ['PHP', 'Laravel', 'CSS', 'Docker', 'HTML'],
			image: {
				href: 'https://i.imgur.com/Uy4V2ma.png',
				local: ''
			},
			href: 'https://github.com/luis-viegas/Protein-Gram'
		}
	];

	function getAllTechnologies() {
		const technologies = [];
		projectData.forEach((project) => {
			project.technologies.forEach((technology) => {
				if (!technologies.includes(technology)) {
					technologies.push(technology);
				}
			});
		});
		return technologies;
	}

	$: technologies = getAllTechnologies();
	let filterTechnologies = [];
</script>

<div id="projects">
	<h1 class="font-bold text-5xl lg:text-8xl mb-3">All Projects</h1>
	<div class="flex items-center mb-6">
		<div class="relative w-full mr-3">
			<div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
				<svg
					aria-hidden="true"
					class="w-5 h-5 lg:w-6 lg:h-6 text-white"
					fill="currentColor"
					viewBox="0 0 20 20"
					xmlns="http://www.w3.org/2000/svg"
					><path
						fill-rule="evenodd"
						d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
						clip-rule="evenodd"
					/></svg
				>
			</div>
			<input
				type="text"
				id="simple-search"
				class="bg-gray-600 lg:text-xl placeholder-gray-300 text-white text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
				placeholder="Search for a project..."
				autocomplete="off"
				bind:value={searchTerm}
			/>
		</div>
		<FilterModal bind:filterTechnologies {technologies} />
	</div>
	{#if filterTechnologies.length != 0}
		<div class="mb-4">
			<h4 class="lg:text-xl">Searching for:</h4>

			{#each filterTechnologies as technology}
				<!-- svelte-ignore a11y-click-events-have-key-events -->
				<div
					class="inline-block cursor-pointer relative"
					on:click={() => {
						filterTechnologies = filterTechnologies.filter((t) => t !== technology);
					}}
				>
					<TechBadge text={technology} />
				</div>
			{/each}
		</div>
	{/if}
	<div class="flex flex-col space-y-4 lg:grid lg:grid-cols-2 lg:space-y-0 lg:gap-8">
		{#each filteredProjects as project (project.id)}
			<ProjectCard {project} />
		{/each}
	</div>
</div>
