<script>
    // @ts-nocheck

	let skills = ['JavaScript', 'Svelte', 'Tailwind CSS', 'HTML', 'CSS'];
	let newSkill = '';

	function addSkill() {
		if (newSkill.trim() !== '') {
			skills = [...skills, newSkill.trim()];
			newSkill = '';
		}
	}

	function removeSkill(skill) {
		skills = skills.filter((s) => s !== skill);
	}
</script>

<section class="rounded-lg bg-gray-100 p-6 shadow-md">
	<h2 class="mb-4 text-2xl font-bold">My Skills</h2>
	<div class="mb-4">
		<input
			bind:value={newSkill}
			type="text"
			placeholder="Add a new skill"
			class="mr-2 rounded-lg border border-gray-300 p-2"
		/>
		<button on:click={addSkill} class="rounded-lg bg-blue-500 p-2 text-white hover:bg-blue-600">
			Add Skill
		</button>
	</div>
	<ul class="space-y-2">
		{#each skills as skill}
			<li class="flex items-center justify-between rounded-lg bg-white p-2 shadow-sm">
				<span>{skill}</span>
				<button on:click={() => removeSkill(skill)} class="p-1 text-red-500 hover:text-red-700">
					Remove
				</button>
			</li>
		{/each}
	</ul>
</section>
