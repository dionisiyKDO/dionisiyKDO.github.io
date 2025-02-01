<script>
    import { page } from '$app/state';

    const links = [
        { name: 'Home', href: '/' },
        { name: 'Projects', href: '/projects' },
    ];
</script>

<div class="navbar-container">
    <div class="navbar">
        {#each links as link}
            {#if link.href === page.url.pathname}
                <a href={link.href} class="navbar-button navbar-button-selected">{link.name}</a>
            {:else}
                <a href={link.href} class="navbar-button">{link.name}</a>
            {/if}
        {/each}
    </div>
</div>

<style>
</style>