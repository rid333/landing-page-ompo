<script>
    import PageHeader from "$lib/components/pageHeader.svelte";
    import Header from "$lib/assets/permainan1.jpeg";
    import Permainan2 from "$lib/assets/permainan2.jpeg";
    import Permainan3 from "$lib/assets/permainan3.jpeg";
    import Permainan4 from "$lib/assets/permainan4.jpeg";
    import Permainan5 from "$lib/assets/permainan5.jpeg";
    import Permainan6 from "$lib/assets/permainan6.jpeg";
    import Fasilitas from "$lib/assets/fasilitasheader.jpeg";
    import Masjid1 from "$lib/assets/masjid.jpeg";
    import Masjid2 from "$lib/assets/gazebo-masjid2.jpeg";
    import Dewasa1 from "$lib/assets/dewasa5.jpeg";
    import Dewasa2 from "$lib/assets/dewasa7.jpeg";
    import Dewasa3 from "$lib/assets/dewasa8.jpeg";
    import DewasaDepan1 from "$lib/assets/dewasa-depan1.jpeg";
    import DewasaDepan2 from "$lib/assets/dewasa-depan3.jpeg";
    import DewasaAnak from "$lib/assets/dewasa-anak.jpeg";

    const Images = [
        Header,
        Masjid1,
        Permainan2,
        Permainan3,
        Dewasa1,
        Permainan4,
        Permainan5,
        Dewasa2,
        Permainan6,
        Fasilitas,
        Dewasa3,
        Masjid2,
        DewasaDepan1,
        DewasaAnak,
        DewasaDepan2
    ];
</script>

<PageHeader title="GALERI" description="Intip suasana seru dan keindahan Permandian Alam Ompo melalui galeri foto kami. Scroll ke bawah dan rasakan pesonanya sebelum Anda berkunjung!" img={Header} />

<div id="main" class="p-5 py-10 lg:p-10 grid lg:grid-cols-3 gap-10">
  {#each Images as img}
    <img class="w-full h-96 object-cover" src={img} alt="Waterpark">
  {/each}
</div>