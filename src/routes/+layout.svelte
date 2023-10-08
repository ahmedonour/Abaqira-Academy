<script>
	import { fly } from 'svelte/transition';
	import Footer from '../component/Footer.svelte';
	import Nav from '../component/Nav.svelte';

	export let data;
</script>

<div class="app">
	<Nav />
	{#key data.url}
		<main in:fly={{ x: -200, duration: 1000, delay: 1000 }} out:fly={{ x: 200, duration: 1000 }}>
			<slot />
		</main>
	{/key}
	<Footer />
</div>

<style>
	.app {
		display: grid;
		place-items: center;
		max-width: 100vw;
		margin: 0;
		padding: 0;
		overflow-x: hidden;
	}
	main {
		max-width: 100%;
	}
</style>
