<script>
    import Jenisfasilitas from "$lib/components/fasilitas/jenisfasilitas.svelte";
    import PageHeader from "$lib/components/pageHeader.svelte";
    import Header from "$lib/assets/fasilitasheader.jpeg";
    import Dewasa1 from "$lib/assets/dewasa1.jpeg";
    import Dewasa2 from "$lib/assets/dewasa2.jpeg";
    import Dewasa3 from "$lib/assets/dewasa3.jpeg";
    import Anak1 from "$lib/assets/anak.jpeg";
    import Anak2 from "$lib/assets/anak1.jpeg";
    import Anak3 from "$lib/assets/dewasa-anak.jpeg";
    import MataAir1 from "$lib/assets/mataair.jpeg";
    import Gazebo1 from "$lib/assets/gazebo2.jpeg";
    import Gazebo2 from "$lib/assets/gazebo5.jpeg";
    import Masjid1 from "$lib/assets/masjid.jpeg";
    import Masjid2 from "$lib/assets/gazebo-masjid1.jpeg";
    import Masjid3 from "$lib/assets/gazebo-masjid2.jpeg";
    import Toilet1 from "$lib/assets/toilet1.jpeg";
    import Toilet2 from "$lib/assets/toilet3.jpeg";
    import Toilet3 from "$lib/assets/toilet5.jpeg";
    import Kantin1 from "$lib/assets/kantin1.jpeg";
    import Kantin2 from "$lib/assets/gazebo-kantin.jpeg";

    const ImgKolamDewasa = [
        Dewasa1,
        Dewasa2,
        Dewasa3,
    ];

    const ImgKolamAnak = [
        Anak1,
        Anak2,
        Anak3,
    ];

    const ImgMataAir = [
        MataAir1,
        MataAir1,
        MataAir1
    ];

    const ImgGazebo = [
        Gazebo1,
        Gazebo2,
        Gazebo1
    ];

    const ImgMasjid = [
        Masjid1,
        Masjid2,
        Masjid3
    ];

    const ImgToilet = [
        Toilet2,
        Toilet1,
        Toilet3
    ];
    
    const ImgKantin = [
        Kantin1,
        Kantin2,
        Kantin1
    ];

</script>

<PageHeader title="FASILITAS" description="Nikmati berbagai fasilitas kami: kolam renang untuk semua usia, gazebo yang nyaman, kantin dengan hidangan lezat dan terjangkau, serta masjid untuk beribadah. Semuanya ada di sini untuk membuat kunjungan Anda sempurna!" img={Header} />

<div id="main" class="flex flex-col lg:gap-y-10 lg:p-10 bg-slate-50">
  <Jenisfasilitas nama="Kolam Renang Dewasa" gambar={ImgKolamDewasa} deskripsi="Kolam renang yang luas dan nyaman, sempurna untuk berenang santai atau berolahraga. Ketinggian 1,5 M hingga 2 M" />
  <Jenisfasilitas nama="Kolam Renang Anak-anak" gambar={ImgKolamAnak} deskripsi="Kolam renang khusus anak-anak dengan desain yang aman dan menyenangkan." />
  <Jenisfasilitas nama="Sumber Mata Air" gambar={ImgMataAir} deskripsi="Sumber mata air yang jernih dengan dan memiliki nilai-nilai spiritual lokal." />
  <Jenisfasilitas nama="Gazebo" gambar={ImgGazebo} deskripsi="Gazebo yang nyaman untuk bersantai dan menikmati pemandangan sekitar." />
  <Jenisfasilitas nama="Masjid" gambar={ImgMasjid} deskripsi="Masjid yang bersih dan nyaman untuk beribadah." />
  <Jenisfasilitas nama="Toilet" gambar={ImgToilet} deskripsi="Toilet yang bersih dan terawat untuk kenyamanan Anda." />
  <Jenisfasilitas nama="Kantin" gambar={ImgKantin} deskripsi="Kantin dengan berbagai pilihan makanan dan minuman untuk memuaskan selera Anda." />
</div>