<script>
    import PageHeader from "$lib/components/pageHeader.svelte";
    import Header from "$lib/assets/IMG_7009-min.png";
</script>

<PageHeader title="GALERI" description="Intip suasana seru dan keindahan Permandian Alam Ompo melalui galeri foto kami. Scroll ke bawah dan rasakan pesonanya sebelum Anda berkunjung!" img={Header} />

<div id="main" class="p-5 py-10 lg:p-10 grid lg:grid-cols-3 gap-10">
  {#each {length: 15} as img}
    <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
  {/each}
</div>