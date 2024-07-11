<script>
    import { Clock7 } from "lucide-svelte";
    let isOpen = true;
</script>

<nav class="text-white uppercase text-lg font-semibold">
    <div class="absolute p-2">
        Logo
    </div>
    <div class="absolute right-0 p-2 flex gap-x-5">
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
        {:else}\
            Tutup
        {/if}
    </div>
</nav>