<script>
	import Typewriter from 'svelte-typewriter';
	const style = 'inline h-8';
</script>

<Typewriter class="container" mode="#loop" cursor={false}>
	<p data-static class={style}>I'm a</p>
	<p class={style}>Software Engineer</p>
	<p class={style}>Data Scientist</p>
</Typewriter>
