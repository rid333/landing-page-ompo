<script>
    import PageHeader from "$lib/components/pageHeader.svelte";
</script>

<PageHeader title="GALERI" description="Lorem, ipsum dolor sit amet consectetur adipisicing elit. A facere nemo fugit eligendi praesentium molestiae magni rem libero ad, atque debitis, illo quaerat sint neque officia explicabo exercitationem voluptate esse!" img="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" />

<div id="galeri" class="p-10 grid grid-cols-3 gap-10">
  {#each {length: 15} as img}
    <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
  {/each}
</div>