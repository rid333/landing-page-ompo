<script>
  import wave_1 from "$lib/assets/layered-waves-haikei.svg"
  import { MoveRight } from "lucide-svelte";
  import { reveal } from 'svelte-reveal';
</script>

<svelte:head>
  <title>Permandian Alam Ompo</title>
</svelte:head>

<div class="relative font-bold text-white">
  <img class="w-screen h-screen" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
  <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-50">
    <div class="flex pl-10 w-1/2 items-center justify-center h-full flex-col">
      <h1 class="text-5xl pb-5">Selamat Datang di Permandian Alam Ompo</h1>
      <p class="text-lg font-medium">Lorem, ipsum dolor sit amet consectetur adipisicing elit. A facere nemo fugit eligendi praesentium molestiae magni rem libero ad, atque debitis, illo quaerat sint neque officia explicabo exercitationem voluptate esse!</p>
    </div>
  </div>
</div>

<div use:reveal class="relative">
  <img class="w-full h-screen object-cover" src={wave_1} alt="Wave 1">
  <div class="absolute inset-0 h-full w-full p-20 flex flex-col items-center gap-y-10">
    <div class="flex flex-col items-center gap-y-4 text-center">
      <p class="text-4xl font-extrabold">Jelajahi Permandian dan Budaya di <span class="text-sky-600">Permandian Alam Ompo</span></p>
      <p class="text-lg font-medium">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt, odio.</p>
    </div>
    <iframe class="w-[600px] aspect-video" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=z6gedapw4t3xREkr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </div>
</div>


<div use:reveal class="bg-[#0059DD] flex flex-col justify-center items-center h-screen px-20 gap-y-3 text-white">
  <div class="font-extrabold text-5xl">Fasilitas</div>
  <div class="font-medium text-xl pb-10">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Earum minima quos nesciunt, facere iste facilis!</div>
  <div class="flex gap-x-20">
    <div class="flex flex-col w-72 text-black bg-white shadow-2xl">
      <img class="" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
      <div class="p-5">
        <p class="text-2xl font-extrabold">Lorem, ipsum.</p>
        <p class="">Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur, nihil.</p>
      </div>
    </div>
    <div class="flex flex-col w-72 text-black bg-white shadow-2xl">
      <img class="" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
      <div class="p-5">
        <p class="text-2xl font-extrabold">Lorem, ipsum.</p>
        <p class="">Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur, nihil.</p>
      </div>
    </div>
    <div class="flex flex-col w-72 text-black bg-white shadown-2xl">
      <img class="" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
      <div class="p-5">
        <p class="text-2xl font-extrabold">Lorem, ipsum.</p>
        <p class="">Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur, nihil.</p>
      </div>
    </div>

  </div>
  <div class="bg-yellow-500 flex gap-x-5 mt-5 font-bold p-3">
    Baca Selengkapnya
    <MoveRight size="24" />
  </div>
</div>

<div use:reveal class="flex flex-col justify-center items-end text-end px-20 p-52">
  <div class="w-1/2 text-5xl flex flex-col gap-5">
    <div class="font-extrabold">Bosan dengan <span class="px-3 rounded-sm bg-[#0059DD] text-white">Air?</span></div>
    <div class="text-xl font-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, quaerat molestiae ullam repellat fuga veritatis blanditiis natus asperiores. Facere, obcaecatdi</div>
  </div>
</div>

<div use:reveal class="relative text-white text-xl">
  <img class="object-cover w-screen h-[500px]" src="https://happyplayindonesia.com/wp-content/uploads/2024/03/image-15.webp" alt="Waterpark">
  <div class="absolute inset-0 h-full w-full p-20 flex flex-col justify-center items-center gap-y-10 bg-black bg-opacity-50">
    <p class="font-extrabold text-4xl">Waktu Operasi</p>
    <div class="flex gap-x-16">
      <div class="p-5 bg-emerald-600">
        <h1 class="font-extrabold">Buka</h1>
        <p>Senin - Jumat: 08.00 - 17.00</p>
        <p>Sabtu - Minggu: 08.00 - 18.00</p>
      </div>
      <div class="p-5 bg-red-500">
        <h1 class="font-extrabold">Tutup</h1>
        <p>Senin - Jumat: 17.00 - 18.00</p>
        <p>Sabtu - Minggu: 18.00 - 19.00</p>
      </div>
    </div>
  </div>
</div>