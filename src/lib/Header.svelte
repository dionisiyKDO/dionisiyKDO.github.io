<script>
	let links = [
		{ name: 'Home', url: '/' },
		{ name: 'About', url: '/about' },
		{ name: 'Projects', url: '/projects' },
		{ name: 'Contact', url: '/contact' }
	];
</script>

<header class="flex justify-between items-center bg-zinc-900 text-white p-4">
	<h1 class="text-2xl font-bold">Denys Kamiskyi</h1>
	<nav>
		<ul class="flex gap-4 list-none">
			{#each links as link}
				<li >
					<a class="hover:underline" href={link.url}>{link.name}</a>
				</li>
			{/each}
		</ul>
	</nav>
</header>

<style>
</style>

