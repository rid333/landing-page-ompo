<script>
    import { Facebook } from "lucide-svelte";
    import { Instagram } from "lucide-svelte";
    import { Twitter } from "lucide-svelte";
    import { Youtube } from "lucide-svelte";
</script>

<footer class="text-xl flex lg:flex-row flex-col relative bg-slate-100 h-full lg:gap-y-0 gap-y-10 gap-x-20 p-10 lg:p-20">
    <div class="lg:w-1/3 flex flex-col gap-y-5 lg:gap-y-20">
        <div class="flex flex-col gap-y-2">
            <h1 class="text-xl lg:text-2xl font-extrabold">Permandian Alam Ompo</h1>
            <p class="text-sm">MV9J+FWW, Ompo, Kec. Lalabata, Kabupaten Soppeng, Sulawesi Selatan 90814</p>
        </div>
        <div class="flex gap-x-5">
            <a href="https://fb.com" target="_blank">
                <Facebook strokeWidth=2 class="lg:w-6 lg:h-6 h-5 w-5" />
            </a>
            <a href="https://instagram.com" target="_blank">
                <Instagram strokeWidth=2 class="lg:w-6 lg:h-6 h-5 w-5" />
            </a>
            <a href="https://x.com" target="_blank">
                <Twitter strokeWidth=2 class="lg:w-6 lg:h-6 h-5 w-5" />
            </a>
            <a href="https://youtube.com" target="_blank">
                <Youtube strokeWidth=2 class="lg:w-6 lg:h-6 h-5 w-5" />
            </a>
        </div>
    </div>
    <div class="flex lg:flex-row flex-col lg:gap-y-0 gap-y-5 gap-x-20 text-base lg:text-lg justify-around">
        <div>
            <div class="font-extrabold">Menu</div>
            <div class="flex flex-col">
                <a href="/home">Home</a>
                <a href="/fasilitas">Fasilitas</a>
                <a href="/galeri">Galeri</a>
                <a href="makanan-dan-minuman">Makanan & Minuman</a>
                <a href="sejarah-ompo">Sejarah Ompo</a>
            </div>
        </div>
        <div>
            <div class="font-extrabold">Lokasi</div>
            <div>
                <div>MV9J+FWW</div>
                <div>Kel. Ompo</div>
                <div>Kec. Lalabata</div>
                <div>Kab. Soppeng</div>
            </div>
        </div>
        <div>
            <div class="font-extrabold">Waktu Operasi</div>
            <div>
                <div>08:00 - 16:00</div>
                <div>Senin - Minggu</div>
            </div>
        </div>
    </div>
    <div class="absolute left-0 bottom-0 text-xs lg:text-sm lg:px-20 px-10 py-2">Copyright Lorem ipsum dolor sit amet.</div>
</footer>