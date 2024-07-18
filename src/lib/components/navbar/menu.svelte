<script>
    export let open;
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
            name: "Tentang Kami",
            link: "/tentang"
        }
    ];
</script>

{#if open}
<div class="flex flex-col h-screen gap-y-10">
        {#each menus as menu}
            <a class="" href={menu.link}>{menu.name}</a>
        {/each}
    </div>
{/if}