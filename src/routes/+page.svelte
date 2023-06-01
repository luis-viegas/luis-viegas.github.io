<script>
	import Contact from '$lib/components/Contact.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import About from './About.svelte';
	import Hero from './Hero.svelte';
	import MyBackground from './MyBackground.svelte';
	import Projects from './Projects.svelte';
	import StarProjects from './StarProjects.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<div id="main" class="flex justify-center">
	<section class="md:w-3/5 w-4/5 max-w-[1200px] pt-20">
		<Hero />
		<div class="h-48" />
		<About />
		<div class="h-48" />
		<Contact />
		<div class="h-48" />
		<MyBackground />
		<div class="h-48" />
		<StarProjects />
		<div class="h-48" />
		<Projects />
		<div class="h-10" />
		<Footer />
	</section>
</div>

<style>
	#main {
		font-family: Roboto;
	}
</style>
