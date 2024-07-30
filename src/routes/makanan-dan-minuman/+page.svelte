<script>
    import PageHeader from "$lib/components/pageHeader.svelte";
    import KantinImg from "$lib/assets/kantin1-min.png";
    import KantinImg1 from "$lib/assets/gazebo-kantin-min.png";
</script>

<PageHeader title="MAKANAN DAN MINUMAN" description="Permandian Alam Ompo memiliki kantin di dalam dan luar area permandian, siap menyajikan berbagai hidangan lezat kapan saja. Puaskan selera makan Anda tanpa harus jauh-jauh!" img={KantinImg} />

 <div class="p-5 py-10 lg:p-20 flex flex-col gap-y-14" id="main">
  <div class="text-lg lg:text-3xl font-bold mx-auto text-center">Permandian Alam Ompo memiliki kantin di dalam dan luar permandian</div>
  <div class="flex flex-col gap-y-8">
    <div class="bg-[#0059DD] w-fit text-white text-lg lg:text-xl font-bold p-2">Kantin di dalam permandian</div>
    <div class="grid lg:grid-cols-3 gap-x-10 gap-y-10">
      <img class="w-full h-96 object-cover" src={KantinImg} alt="Kantin">
      <img class="w-full h-96 object-cover" src={KantinImg1} alt="Kantin 2">
      <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
    </div>
  </div>
  <div class="flex flex-col gap-y-8">
    <div class="bg-[#0059DD] w-fit text-white text-lg lg:text-xl font-bold p-2">Kantin di luar permandian</div>
    <div class="grid lg:grid-cols-3 gap-x-10 gap-y-10">
      <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
      <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
      <img class="w-full h-96 object-cover" src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1" alt="Waterpark">
    </div>
  </div>
</div>