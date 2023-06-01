<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';

	import Navbar from '$lib/components/Navbar.svelte';
	import Sidebar from '$lib/components/Sidebar.svelte';

	let open = false;

	const desktop_class = 'flex justify-end gap-x-6 pr-20';
	let li_class = 'hover:text-[#151518] hover:bg-white  px-2';
</script>

<nav class="">
	<Sidebar bind:open />
	<Navbar bind:sidebar={open} />
</nav>

<style>
</style>
