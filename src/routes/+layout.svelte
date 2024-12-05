<script>
	import Header from '$lib/components/header/Header.svelte';
	import '../app.css';
	let { children } = $props();
</script>

<div class="min-h-screen dark:bg-zinc-900 dark:text-zinc-50">
	<Header />
	{@render children()}
</div>

