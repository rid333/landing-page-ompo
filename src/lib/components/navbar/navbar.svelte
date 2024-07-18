<script>
    import { Clock7 } from "lucide-svelte";
    import logo from "$lib/assets/logo.png";
    import { Hamburger } from "svelte-hamburgers";
    import Menu from "./menu.svelte";

    import { onMount, onDestroy } from "svelte";
    import { afterUpdate } from 'svelte';
    let open;
    let isOpen = true;
    let isScrolled = false;

        const handleScroll = () => {
        if (typeof window !== 'undefined') {
            isScrolled = window.scrollY > 50;
        }
    };

    onMount(() => {
        if (typeof window !== 'undefined') {
            window.addEventListener('scroll', handleScroll);
        }
    });

    onDestroy(() => {
        if (typeof window !== 'undefined') {
            window.removeEventListener('scroll', handleScroll);
        }
    });

    afterUpdate(() => {
        if (typeof window !== 'undefined') {
            isScrolled = window.scrollY > 50;
        }
    });

    const menus = [
        {
            name: "Home",
            link: "/"
        },
        {
            name: "Fasilitas",
            link: "/fasilitas"
        },
        {
            name: "Galeri",
            link: "/galeri"
        },
        {
            name: "Makanan & Minuman",
            link: "/makanan-dan-minuman"
        },
        {
            name: "Sejarah Ompo",
            link: "/sejarah-ompo"
        }
    ];
</script>

<nav class={`p-2 lg:p-4 text-white flex justify-between items-center w-full fixed top-0 left-0 z-50 uppercase text-base font-semibold transition-colors duration-300 bg-gray-800/75 ${isScrolled ? "lg:bg-gray-800/75" : ""}`}>
    <a href="/" class="lg:block hidden">
        <img class="w-12" src={logo} alt="Logo">
    </a>
    <div class="lg:flex hidden gap-x-5">
        {#each menus as {name, link} (name)}
            <a href={link}>{name}</a>
        {/each}
        {#if isOpen}
            <div class="flex gap-x-1.5 text-xs items-center bg-emerald-600 px-1.5 py-1">
                <p>Buka</p>
                <div class="flex gap-x-1 items-center">
                    <Clock7 size="14" />
                    08:00 - 16.00
                </div>
            </div>
        {:else}
            <div class="flex gap-x-1.5 text-xs items-center bg-red-500 px-1.5 py-1">
                <p>Tutup</p>
                <div class="flex gap-x-1 items-center">
                    <Clock7 size="14" />
                    16:00 - 8.00
                </div>
            </div>
        {/if}
    </div>
    <div class="lg:hidden">
        <Hamburger bind:open />
        <Menu bind:open />
    </div> 
</nav>
