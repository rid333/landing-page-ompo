<script>
    import { Clock7 } from "lucide-svelte";
    import { onMount, onDestroy } from "svelte";
    import { afterUpdate } from 'svelte';
    let isOpen = true;
    let isScrolled = false;

        const handleScroll = () => {
        if (typeof window !== 'undefined') {
            isScrolled = window.scrollY > 50;
        }
    };

    onMount(() => {
        if (typeof window !== 'undefined') {
            window.addEventListener('scroll', handleScroll);
        }
    });

    onDestroy(() => {
        if (typeof window !== 'undefined') {
            window.removeEventListener('scroll', handleScroll);
        }
    });

    afterUpdate(() => {
        if (typeof window !== 'undefined') {
            isScrolled = window.scrollY > 50;
        }
    });
</script>

<nav class={`p-4 text-white flex justify-between w-full fixed top-0 left-0 z-50 uppercase text-base font-semibold transition-colors duration-300 ${isScrolled ? "bg-gray-800/75" : ""}`}>
    <div>
        Logo
    </div>
    <div class="flex gap-x-5">
        <a href="/">Home</a>
        <a href="/">Fasilitas</a>
        <a href="/">Galeri</a>
        <a href="/">Makanan & Minuman</a>
        <a href="/">Tentang Kami</a>
        {#if isOpen}
            <div class="flex gap-x-1.5 text-xs items-center bg-emerald-600 px-1.5 py-1">
                <p>Buka</p>
                <div class="flex gap-x-1 items-center">
                    <Clock7 size="14" />
                    08:00 - 16.00
                </div>
            </div>
        {:else}
            <div class="flex gap-x-1.5 text-xs items-center bg-red-500 px-1.5 py-1">
                <p>Tutup</p>
                <div class="flex gap-x-1 items-center">
                    <Clock7 size="14" />
                    16:00 - 8.00
                </div>
            </div>
        {/if}
    </div>
</nav>