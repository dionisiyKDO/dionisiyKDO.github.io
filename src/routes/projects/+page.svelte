<script>
    import avatar from '$lib/assets/avatar.webp';
</script>

<div class="avatar-container">
    <img src={avatar} alt="A beautiful sunset" class="avatar">
</div>

{#each [1, 2] as block}
    <div class="block">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil, qui magnam? Fuga, possimus, eveniet quis accusamus quidem praesentium harum ipsam dolor voluptatum voluptate molestiae reiciendis est rem reprehenderit ullam nihil.    
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta deserunt illo, sequi dignissimos similique tenetur consequatur est harum et incidunt reprehenderit ex omnis doloremque rem voluptates laudantium necessitatibus, fuga corrupti?
    </div>
{/each}

