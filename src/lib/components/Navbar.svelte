<script>
	import Hamburger from './Hamburger.svelte';
	import Menu from './Menu.svelte';

	export let sidebar = false;
</script>

<header class="flex justify-between p-8 items-center md:justify-end text-white">
	<Hamburger bind:open={sidebar} />

	<Menu />
</header>
