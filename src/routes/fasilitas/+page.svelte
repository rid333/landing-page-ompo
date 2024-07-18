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
  <Jenisfasilitas nama="Kolam Renang Dewasa" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman, sempurna untuk berenang santai atau berolahraga. Ketinggian 1,5 M hingga 2 M" />
  <Jenisfasilitas nama="Kolam Renang Anak-anak" gambar={ImgKolamDewase} deskripsi="Kolam renang khusus anak-anak dengan desain yang aman dan menyenangkan." />
  <Jenisfasilitas nama="Sumber Mata Air" gambar={ImgKolamDewase} deskripsi="Sumber mata air yang jernih dengan dan memiliki nilai-nilai spiritual lokal." />
  <Jenisfasilitas nama="Gazebo" gambar={ImgKolamDewase} deskripsi="Gazebo yang nyaman untuk bersantai dan menikmati pemandangan sekitar." />
  <Jenisfasilitas nama="Masjid" gambar={ImgKolamDewase} deskripsi="Masjid yang bersih dan nyaman untuk beribadah." />
  <Jenisfasilitas nama="Toilet" gambar={ImgKolamDewase} deskripsi="Toilet yang bersih dan terawat untuk kenyamanan Anda." />
  <Jenisfasilitas nama="Kantin" gambar={ImgKolamDewase} deskripsi="Kantin dengan berbagai pilihan makanan dan minuman untuk memuaskan selera Anda." />
</div>