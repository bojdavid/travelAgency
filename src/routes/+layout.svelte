<script lang="ts">
  //import "../../src/lib/styles/app.css";
  import "../lib/styles/app.css";
  import Nav from "../lib/components/navigation/Nav.svelte";
  import Footer from "../lib/components/navigation/Footer.svelte";
  let { children } = $props();
</script>

<header class="mt-10 font-hanken flex justify-between mx-20">
  <div></div>
  <div>
    <Nav />
  </div>
  <div>flag</div>
</header>
<main class="mx-20 font-hanken">
  {@render children()}
</main>
<footer>
  <div class="mx-auto w-4xl mb-20">
    <Footer />
  </div>
</footer>

<style>
  :global(.light-font) {
    font-weight: 400;
  }
</style>
