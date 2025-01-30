<script>
	import Header from '$lib/Header.svelte';
	import About from '$lib/About.svelte';
	import Projects from '$lib/Projects.svelte';
	import Footer from '$lib/Footer.svelte';
	import Skills from '$lib/Skills.svelte';
</script>

<div class="flex min-h-screen flex-col">
	<Header />
	<main class="flex-grow p-6">
		<About />
		<Projects />
		<Skills />
	</main>
	<Footer />
</div>

<style>
</style>
