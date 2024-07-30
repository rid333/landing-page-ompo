<script>
  import wave_1 from "$lib/assets/layered-waves-haikei.svg";
  import Fasilitas from "$lib/components/home/fasilitas.svelte";
  import Header from "$lib/assets/dewasa-depan-min.png";
  import AnakImg from "$lib/assets/anak.png";
  import MataAirImg from "$lib/assets/mataair.png";
  import DewasaImg from "$lib/assets/dewasa3.png";
  import { ChevronDown } from "lucide-svelte";
  import Carousel from 'svelte-carousel';
  import { MoveRight } from "lucide-svelte";
</script>

<svelte:head>
  <title>Permandian Alam Ompo</title>
</svelte:head>

<div class="relative font-bold text-white">
  <img class="w-screen h-screen object-cover" src={Header} alt="Waterpark">
  <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-50">
    <div class="flex pl-10 w-2/3 lg:w-1/2 items-center justify-center h-full flex-col">
      <h1 class="text-3xl lg:text-5xl pb-5 uppercase">Selamat Datang di Permandian Alam Ompo</h1>
      <p class="text-sm lg:text-lg font-medium italic">Nikmati pengalaman tak terlupakan dengan permandian alam yang segar, budaya lokal yang kaya, dan edukasi menarik di Permandian Alam Ompo.</p>
    </div>
  </div>
  <a href="#home" class="absolute bottom-0 left-1/2 right-1/2 animate-bounce">
    <ChevronDown size="64" />
  </a>
</div>

<div id="home" class="relative">
  <img class="w-full h-screen object-cover" src={wave_1} alt="Wave 1">
  <div class="absolute inset-0 h-full p-5 lg:p-20 flex flex-col items-center justify-center lg:gap-y-10 gap-y-20">
    <div class="flex flex-col items-center gap-y-10 lg:gap-y-4 text-center">
      <p class="text-2xl lg:text-4xl font-extrabold">Jelajahi Permandian dan Budaya di <span class="text-sky-600">Permandian Alam Ompo</span></p>
      <p class="text-base lg:text-lg font-medium">Bukan hanya permandian yang menyegarkan, di sini Anda juga bisa menemukan sejarah yang kaya dan edukasi yang menarik</p>
    </div>
    <iframe class="w-[300px] lg:w-[600px] aspect-video" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=z6gedapw4t3xREkr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </div>
</div>

<div class="bg-[#0059DD] flex flex-col justify-center items-center h-full p-5 py-10 lg:p-20 gap-y-5 text-white">
  <div class="font-extrabold text-4xl lg:text-5xl">Fasilitas</div>
  <div class="font-medium text-base text-center italic lg:text-xl pb-10">Kami menawarkan tiga fasilitas permandian utama, yaitu Kolam Renang Dewasa, Kolam Renang Anak-anak, dan Sumber Mata Air</div>
  <div class="flex lg:flex-row flex-col gap-x-20 gap-y-10">
    <Fasilitas title="Kolam Renang Dewasa" image={DewasaImg} description="Kolam renang yang luas dan nyaman, sempurna untuk berenang santai atau berolahraga. Ketinggian 1,5 M hingga 2 M" />
    <Fasilitas title="Kolam Renang Anak-anak" image={AnakImg} description="Kolam renang khusus anak-anak dengan desain yang aman dan menyenangkan." />
    <Fasilitas title="Sumber Mata Air" image={MataAirImg} description="Sumber mata air yang jernih dengan dan memiliki nilai-nilai spiritual lokal." />
  </div>
  <a href="/fasilitas" class="bg-yellow-500 flex gap-x-5 mt-5 font-bold p-3">
    Baca Selengkapnya
    <MoveRight size="24" />
  </a>
</div>

<div class="flex flex-col-reverse lg:flex-row justify-center items-center lg:text-end p-5 py-10 lg:p-20 gap-x-10">
  <div class="mt-5 lg:pt-0 w-[400px] lg:w-[600px]">
    <Carousel>
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
    </Carousel>
  </div>
  <div class="lg:w-1/2 text-2xl lg:text-5xl flex flex-col gap-5">
    <div class="font-extrabold">Bosan dengan <span class="px-3 rounded-sm bg-[#0059DD] text-white">Air?</span></div>
    <div class="italic text-base lg:text-xl font-medium">Pindai QR Code di poster dekat mata air untuk mempelajari sejarah unik Permandian Alam Ompo. Jangan lewatkan juga kesempatan belajar tentang berbagai jenis pohon di sini melalui display yang tersedia di depan pohon.</div>
  </div>
</div>


<div class="flex flex-col lg:flex-row justify-center items-center lg:text-start p-5 py-10 lg:p-20 gap-x-10">
  <div class="lg:w-1/2 text-2xl lg:text-5xl flex flex-col gap-5">
    <div class="font-extrabold">Lelah? Ingin <span class="px-3 rounded-sm bg-[#0059DD] text-white">Istirahat?</span></div>
    <div class="italic text-base lg:text-xl font-medium">Permandian Alam Ompo menawarkan berbagai jenis gazebo yang nyaman untuk beristirahat. Temukan gazebo favoritmu dan nikmati suasana di Permandian Alam Ompo.</div>
  </div>
  <div class="mt-5 lg:pt-0 w-[400px] lg:w-[600px]">
    <Carousel>
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
    </Carousel>
  </div>
</div>

<div class="flex flex-col-reverse lg:flex-row justify-center items-center lg:text-end p-5 py-10 lg:p-20 gap-x-10">
  <div class="mt-5 lg:pt-0 w-[400px] lg:w-[600px]">
    <Carousel>
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
      <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Test" class="object-cover" />
    </Carousel>
  </div>
  <div class="lg:w-1/2 text-2xl lg:text-5xl flex flex-col gap-5">
    <div class="font-extrabold">Lapar? Pengen <span class="px-3 rounded-sm bg-[#0059DD] text-white">Ngemil?</span></div>
    <div class="italic text-base lg:text-xl font-medium">Jangan lewatkan kantin-kantin yang menyajikan berbagai pilihan makanan lezat dengan harga terjangkau. Nikmati hidangan favoritmu setelah berendam!</div>
  </div>
</div>

<div class="flex flex-col justify-center text-center p-5 py-10 lg:p-20 bg-[#0059DD] text-white">
  <div class="text-2xl lg:text-5xl flex flex-col justify-center items-center gap-5">
    <div class="font-extrabold italic">Come and Have Fun with Us</div>
    <div class="text-base lg:text-xl font-medium">MV9J+FWW, Ompo, Kec. Lalabata, Kabupaten Soppeng, Sulawesi Selatan 90814</div>
    <iframe class="lg:w-[450px] h-96" title="Permandian Alam Ompo" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3978.4237062468465!2d119.87976447443778!3d-4.331260395642732!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2d95f6a0b2ca6a7b%3A0x4b8ba8fc531b5b81!2sPermandian%20Alam%20Ompo!5e0!3m2!1sid!2sid!4v1721176773241!5m2!1sid!2sid" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
  </div>
</div>

<div class="relative text-white text-base lg:text-xl">
  <img class="object-cover w-screen h-[500px]" src="https://happyplayindonesia.com/wp-content/uploads/2024/03/image-15.webp" alt="Waterpark">
  <div class="absolute inset-0 h-full w-full p-10 lg:p-20 flex flex-col justify-center items-center gap-y-10 bg-black bg-opacity-50">
    <p class="font-extrabold text-3xl lg:text-4xl">Waktu Operasi</p>
    <div class="flex lg:flex-row flex-col gap-x-16 gap-y-10">
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