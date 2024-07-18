<script>
    import Carousel from 'svelte-carousel';
    export let nama, gambar, deskripsi;
</script>

<div class="px-20 flex justify-between items-center gap-x-5">
    <div class="flex flex-col gap-y-5">
        <div class="text-3xl font-bold"><span class="bg-sky-600 text-white p-2">{nama}</span></div>
        <div class="text-xl font-medium italic">{deskripsi}</div>
    </div>
    <div class="w-[700px]">
        <Carousel>
            {#each gambar as gambar}
                <img src={gambar} alt={nama} class="object-cover" />
            {/each}
        </Carousel>
    </div>
</div>