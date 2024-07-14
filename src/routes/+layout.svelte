<script>
  import "../app.css";
  import Navbar from "$lib/components/navbar/navbar.svelte";
  import Footer from "$lib/components/footer/footer.svelte";
</script>

<div>
  <Navbar />
  <slot />
  <Footer />
</div>