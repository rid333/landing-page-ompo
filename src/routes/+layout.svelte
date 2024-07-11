<script>
  import "../app.css";
  import Navbar from "$lib/components/navbar/navbar.svelte";
  import IsOpen from "$lib/components/navbar/openornot.svelte";
</script>

<!-- <IsOpen /> -->
<Navbar />
<slot />