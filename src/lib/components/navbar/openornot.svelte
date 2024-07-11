<script>
    import { Clock7 } from "lucide-svelte";

    let isOpen = true;
</script>

<div class="text-sm">
{#if isOpen}
    <div class="flex text-white items-center gap-x-5 font-semibold justify-end p-1.5 bg-emerald-600">
        <p>Buka</p>
        <p class="flex gap-x-1.5 px-2 p-0.5 items-center">
            <Clock7 size="16" />
            08:00 - 16.00
        </p>
    </div>
{:else}
    <div class="flex text-white items-center gap-x-5 font-semibold justify-end p-1.5 bg-red-600">
        <p>Tutup</p>
        <p class="flex gap-x-1.5 px-2 p-0.5 items-center">
            <Clock7 size="20" />
            16:00 - 08.00
        </p>
    </div>
{/if}
</div>