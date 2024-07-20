<script>
    export let open;
    import { fly } from 'svelte/transition';

    const menus = [
        {
            name: "Home",
            link: "/"
        },
        {
            name: "Fasilitas",
            link: "/fasilitas"
        },
        {
            name: "Galeri",
            link: "/galeri"
        },
        {
            name: "Makanan & Minuman",
            link: "/makanan-dan-minuman"
        },
        {
            name: "Sejarah Ompo",
            link: "/sejarah-ompo"
        }
    ];
</script>

{#if open}
<div class="flex flex-col h-screen gap-y-10 p-5">
    {#each menus as menu, i}
        <a class="" href={menu.link} transition:fly={{ y: -15, delay: 50 * i }}>{menu.name}</a>
    {/each}
</div>
{/if}
