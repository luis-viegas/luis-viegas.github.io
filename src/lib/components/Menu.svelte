<script>
	import { page } from '$app/stores';
	let li_class = 'hover:text-[#151518] hover:bg-white  px-2';
</script>

<nav class="uppercase text-bold sm:block md:block hidden">
	<ul class="flex justify-end gap-x-6 pr-20">
		<li class={li_class}>
			<a href="#about">About</a>
		</li>
		<li class={li_class}>
			<a href="#contacts">Contacts</a>
		</li>
		<li class={li_class}>
			<a href="#background">Background</a>
		</li>
		<li class={li_class}>
			<a href="#projects">Projects</a>
		</li>
	</ul>
</nav>
