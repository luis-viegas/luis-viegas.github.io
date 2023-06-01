<script>
	import Nav from './Nav.svelte';
	import '../app.css';
</script>

<div class="bg-[#151518] text-white ">
	<Nav />

	<main>
		<slot />
	</main>
</div>
