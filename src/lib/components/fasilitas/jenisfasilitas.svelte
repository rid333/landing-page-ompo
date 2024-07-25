<script>
    import Carousel from 'svelte-carousel';
    export let nama, gambar, deskripsi;
</script>

<div class="p-5 py-10 lg:p-20 flex flex-col lg:flex-row justify-between items-center gap-y-5 gap-x-5">
    <div class="flex flex-col gap-y-5 lg:gap-y-5">
        <div class="text-xl lg:text-3xl font-bold"><span class="bg-sky-600 text-white p-2">{nama}</span></div>
        <div class="text-base lg:text-xl font-medium italic">{deskripsi}</div>
    </div>
    <div class="w-[400px] lg:w-[700px]">
        <Carousel>
            {#each gambar as gambar}
                <img src={gambar} alt={nama} class="object-cover" />
            {/each}
        </Carousel>
    </div>
</div>