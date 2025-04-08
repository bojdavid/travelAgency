<script lang="ts">
  import "../lib/styles/app.css";
  let { children } = $props();
</script>

<header></header>
<main>
  {@render children()}
</main>
<footer>footer</footer>
