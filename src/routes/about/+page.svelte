<script>
	let counter = 0;
</script>

<div class="flex items-center justify-center flex-col space-y-6">
	<p class="text-3xl font-medium text-blue-500 capitalize text-center">hello this is about page</p>
	{#if counter > 0}
		<p class="text-3xl">Current value is <span class="text-red-500">{counter}</span></p>
	{/if}
	<button
		on:click={() => (counter += 1)}
		class="bg-gray-200 text-black px-5 py-2 border-black border-2 border-b-4 capitalize shadow-md transition-all duration-300"
		>increment</button
	>
</div>
