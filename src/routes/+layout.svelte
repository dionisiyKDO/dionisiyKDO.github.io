<script lang="ts">
	import Header from '$lib/Header.svelte';
	import Footer from '$lib/Footer.svelte';
	import Navbar from '$lib/Navbar.svelte';
	import '../app.css';
	let { children } = $props();
</script>


<div class="flex min-h-screen flex-col items-center">
	<!-- <Header /> -->
	<main class="flex-grow">
		{@render children()}
		<Navbar />
	</main>
	
	<!-- <Footer /> -->
</div>


<style>
</style>


