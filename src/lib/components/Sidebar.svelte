<script lang="ts">
	export let open = false;

	import { onMount } from 'svelte';

	$: document.body.style.overflow = open ? 'hidden' : 'auto';

	function handleAnchorClick(event) {
		open = false;
		event.preventDefault();
		const link = event.currentTarget;
		const anchorId = new URL(link.href).hash.replace('#', '');
		const anchor = document.getElementById(anchorId);
		window.scrollTo({
			top: anchor.offsetTop,
			behavior: 'smooth'
		});
	}
</script>

<aside class="absolute w-full h-full bg-[#000000ed] flex items-center justify-center " class:open>
	<nav class="text-6xl">
		<a class="block mb-8 hover:text-gray-400" on:click={handleAnchorClick} href="#about">About</a>
		<a class="block mb-8 hover:text-gray-400" on:click={handleAnchorClick} href="#contact"
			>Contact</a
		>
		<a class="block mb-8 hover:text-gray-400" on:click={handleAnchorClick} href="#background"
			>Background</a
		>
		<a class="block mb-8 hover:text-gray-400" on:click={handleAnchorClick} href="#projects"
			>Projects</a
		>
	</nav>
</aside>

<style>
	aside {
		left: -100%;
		transition: left 0.3s ease-in-out;
	}

	.open {
		left: 0;
	}
</style>
