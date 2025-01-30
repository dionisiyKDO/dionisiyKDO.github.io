<script>
	let projects = [
		{ name: 'Project 1', description: 'A brief description of Project 1.', url: '#' },
		{ name: 'Project 2', description: 'A brief description of Project 2.', url: '#' },
		{ name: 'Project 3', description: 'A brief description of Project 3.', url: '#' }
	];
</script>

<section class="rounded-lg bg-gray-100 p-6 shadow-md m-6">
	<h2 class="mb-4 text-2xl font-bold">My Projects</h2>
	<ul class="space-y-2">
		{#each projects as project}
			<li class="flex items-center justify-between rounded-lg bg-white p-2 shadow-sm">
				<h3 class="text-lg font-medium">{project.name}</h3>
				<p class="text-sm">{project.description}</p>
				<a href={project.url} class="p-1 text-blue-500 hover:text-blue-700">Learn More</a>
			</li>
		{/each}
	</ul>
</section>

<style>
</style>
