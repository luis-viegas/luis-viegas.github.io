<script>
	export let text;
</script>

<div class="inline-block">
	{#if ['React', 'PHP'].includes(text)}
		<span
			class="bg-blue-100 lg:text-sm text-blue-800 text-[0.65rem] font-medium mr-2 px-2.5 py-0.5 rounded dark:bg-blue-900 dark:text-blue-300"
			>{text}</span
		>
	{:else if ['JavaScript'].includes(text)}
		<span
			class="bg-red-100 lg:text-sm text-red-800 text-[0.65rem] font-medium mr-2 px-2.5 py-0.5 rounded dark:bg-red-900 dark:text-red-300"
			>{text}</span
		>
	{:else}
		<span
			class="bg-gray-100  lg:text-sm text-gray-800 text-[0.65rem] font-medium mr-2 px-2.5 py-0.5 rounded dark:bg-gray-700 dark:text-gray-300"
			>{text}</span
		>
	{/if}
</div>
