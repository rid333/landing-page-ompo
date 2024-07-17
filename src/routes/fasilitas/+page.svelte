<script>
    import { ChevronDown } from "lucide-svelte";
    import Jenisfasilitas from "$lib/components/fasilitas/jenisfasilitas.svelte";
    const ImgKolamDewase = [
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
    ];
</script>


<div class="relative font-bold text-white">
  <img class="w-screen h-screen" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
  <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-50">
    <div class="flex px-72 items-center justify-center text-justify h-full flex-col">
      <h1 class="text-5xl pb-5">FASILITAS</h1>
      <p class="text-lg font-medium">Lorem, ipsum dolor sit amet consectetur adipisicing elit. A facere nemo fugit eligendi praesentium molestiae magni rem libero ad, atque debitis, illo quaerat sint neque officia explicabo exercitationem voluptate esse!</p>
    </div>
  </div>
  <a href="#fasilitas" class="absolute bottom-0 left-1/2 right-1/2 animate-bounce">
    <ChevronDown size="64" />
  </a>
</div>

<div id="fasilitas" class="flex flex-col gap-y-10 p-10 bg-slate-50">
  <Jenisfasilitas nama="Kolam Renang Dewasa" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Kolam Renang Anak-anak" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Sumber Mata Air" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Gazebo" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Masjid" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Toilet" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
  <Jenisfasilitas nama="Kantin" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman" />
</div>