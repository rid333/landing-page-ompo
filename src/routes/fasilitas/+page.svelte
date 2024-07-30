<script>
    import Jenisfasilitas from "$lib/components/fasilitas/jenisfasilitas.svelte";
    import PageHeader from "$lib/components/pageHeader.svelte";
    import Header from "$lib/assets/fasilitasheader.png";
    const ImgKolamDewase = [
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
        "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/c9/32/2b/flamingo-waterpark-resort.jpg?w=1200&h=-1&s=1",
    ];
</script>

<PageHeader title="FASILITAS" description="Nikmati berbagai fasilitas kami: kolam renang untuk semua usia, gazebo yang nyaman, kantin dengan hidangan lezat dan terjangkau, serta masjid untuk beribadah. Semuanya ada di sini untuk membuat kunjungan Anda sempurna!" img={Header} />

<div id="main" class="flex flex-col lg:gap-y-10 lg:p-10 bg-slate-50">
  <Jenisfasilitas nama="Kolam Renang Dewasa" gambar={ImgKolamDewase} deskripsi="Kolam renang yang luas dan nyaman, sempurna untuk berenang santai atau berolahraga. Ketinggian 1,5 M hingga 2 M" />
  <Jenisfasilitas nama="Kolam Renang Anak-anak" gambar={ImgKolamDewase} deskripsi="Kolam renang khusus anak-anak dengan desain yang aman dan menyenangkan." />
  <Jenisfasilitas nama="Sumber Mata Air" gambar={ImgKolamDewase} deskripsi="Sumber mata air yang jernih dengan dan memiliki nilai-nilai spiritual lokal." />
  <Jenisfasilitas nama="Gazebo" gambar={ImgKolamDewase} deskripsi="Gazebo yang nyaman untuk bersantai dan menikmati pemandangan sekitar." />
  <Jenisfasilitas nama="Masjid" gambar={ImgKolamDewase} deskripsi="Masjid yang bersih dan nyaman untuk beribadah." />
  <Jenisfasilitas nama="Toilet" gambar={ImgKolamDewase} deskripsi="Toilet yang bersih dan terawat untuk kenyamanan Anda." />
  <Jenisfasilitas nama="Kantin" gambar={ImgKolamDewase} deskripsi="Kantin dengan berbagai pilihan makanan dan minuman untuk memuaskan selera Anda." />
</div>