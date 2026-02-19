<script lang="ts">
	import Header from "../components/Header.svelte";
	import favicon from '$lib/assets/favicon.svg';
	let { children } = $props();
	import "../app.css"
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="fixed top-0 left-0 w-full z-50">
	<Header/>
</div>

{@render children()}
