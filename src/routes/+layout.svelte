<script>
	import Footer from '$lib/components/footer/Footer.svelte';
	import Header from '$lib/components/header/Header.svelte';
	import '../app.css';
	let { children } = $props();
</script>

<div class="min-h-screen flex flex-col dark:bg-zinc-900 dark:text-zinc-50">
	<Header />
	<main class="flex-1">{@render children()}</main>
	<Footer />
</div>

