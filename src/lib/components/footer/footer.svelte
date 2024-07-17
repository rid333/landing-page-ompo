<script>
    import { Facebook } from "lucide-svelte";
    import { Instagram } from "lucide-svelte";
    import { Twitter } from "lucide-svelte";
    import { Youtube } from "lucide-svelte";
    import { reveal } from 'svelte-reveal';
</script>

<footer use:reveal class="text-xl flex relative bg-slate-100 h-full gap-x-20 p-20">
    <div class="w-1/3 flex flex-col gap-y-20">
        <div class="flex flex-col gap-y-2">
            <h1 class="text-2xl font-extrabold">Permandian Alam Ompo</h1>
            <p class="text-sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="flex gap-x-5">
            <a href="https://fb.com" target="_blank">
                <Facebook strokeWidth=2 class="w-6 h-6" />
            </a>
            <a href="https://instagram.com" target="_blank">
                <Instagram strokeWidth=2 class="w-6 h-6" />
            </a>
            <a href="https://x.com" target="_blank">
                <Twitter strokeWidth=2 class="w-6 h-6" />
            </a>
            <a href="https://youtube.com" target="_blank">
                <Youtube strokeWidth=2 class="w-6 h-6" />
            </a>
        </div>
    </div>
    <div class="flex gap-x-20 text-lg justify-around">
        <div>
            <div class="font-extrabold">Menu</div>
            <div>
                <div>Home</div>
                <div>Fasilitas</div>
                <div>Galeri</div>
                <div>Makanan & Minuman</div>
                <div>Tentang Kami</div>
            </div>
        </div>
        <div>
            <div class="font-extrabold">Lokasi</div>
            <div>
                <div>Jl. Lorem, ipsum.</div>
                <div>Kel. Lorem.</div>
                <div>Kec. Lorem.</div>
                <div>Kab. Lorem.</div>
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
    <div class="absolute left-0 bottom-0 text-sm px-20 py-2">Copyright Lorem ipsum dolor sit amet.</div>
</footer>