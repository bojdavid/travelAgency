<script lang="ts">
  //import "../../src/lib/styles/app.css";
  import "../lib/styles/app.css";
  let { children } = $props();
  interface navigation {
    nav: String;
    url: string;
  }
  //let navs: string[] = ["Home", "Booking", "Contact Us", "Pricing"];
  let navs: navigation[] = [
    { nav: "Home", url: "/" },
    { nav: "Bookings", url: "/bookings" },
    { nav: "Contact Us", url: "/contact_us" },
    { nav: "Pricing", url: "/pricing" },
  ];
</script>

<header class="mt-10">
  <nav class="bg-stone-950 text-stone-100 w-xl mx-auto rounded-full p-5 flex">
    <ul class="flex justify-evenly items-center">
      {#each navs as nav}
        <li class="capitalize text-lg">
          <a href={nav.url}>
            {nav.nav}
          </a>
        </li>
      {/each}
    </ul>
    <a href="/bookATrip" class="p-4 bg-stone-300 justify-end">Book A Trip</a>
  </nav>
</header>
<main>
  {@render children()}
</main>
<footer>footer</footer>
