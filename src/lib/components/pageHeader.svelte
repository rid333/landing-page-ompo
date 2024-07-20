<script>
    import { ChevronDown } from "lucide-svelte";
    export let title, description, img;
</script>

<div class="relative font-bold text-white">
  <img class="w-screen h-screen" src={img} alt="Waterpark">
  <div class="absolute top-0 left-0 w-full h-full bg-black bg-opacity-50">
    <div class="flex px-11 lg:px-72 items-center justify-center text-justify h-full flex-col">
      <h1 class="text-3xl lg:text-5xl pb-2.5 lg:pb-5">{title}</h1>
      <p class="text-base italic lg:text-lg font-medium">{description}</p>
    </div>
  </div>
  <a href="#fasilitas" class="absolute bottom-0 left-1/2 right-1/2 animate-bounce">
    <ChevronDown size="64" />
  </a>
</div>