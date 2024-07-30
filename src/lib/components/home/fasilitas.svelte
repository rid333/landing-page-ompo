<script>
    export let title, image, description;
</script>

<div class="flex flex-col w-72 lg:w-72 text-black bg-white shadow-2xl">
    <img class="object-cover h-56" src={image} alt="Ompo">
    <div class="p-5 flex flex-col gap-y-2">
        <p class="text-lg lg:text-2xl font-extrabold">{title}</p>
        <p class="text-sm lg:text-base">{description}</p>
    </div>
</div>