<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
	<link href="https://fonts.googleapis.com/css2?family=Cascadia+Mono:ital,wght@0,200..700;1,200..700&display=swap" rel="stylesheet">

	<link rel="icon" href={favicon} />

</svelte:head>

{@render children()}

<style>
	:global(body) {
		background-color: #f0f0f0;
		color: #333;
		font-family: 'Cascadia Mono', monospace;
		margin: 0;
	}
	:global(html) {
	scroll-behavior: smooth;
	}
</style>
