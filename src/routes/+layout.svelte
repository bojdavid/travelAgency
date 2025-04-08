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

<header class="mt-10 font-hanken">
  <div class="flex justify-center">
    <div class="w-[90px]">
      <p class="text-[24px] mx-auto font-sofia font-weight-400">
        Soar (::) Travels
      </p>
    </div>
    <nav
      class="bg-stone-950 text-stone-100 w-[540px] rounded-full py-[7px] pr-[6px] pl-[20px] flex justify-between text-lg"
    >
      <ul class="flex justify-evenly gap-5 items-center">
        {#each navs as nav}
          <li class="">
            <a href={nav.url}>
              {nav.nav}
            </a>
          </li>
        {/each}
      </ul>
      <a
        href="/bookATrip"
        class="py-2 px-6 bg-stone-50 justify-end text-stone-950 rounded-full"
        ><span class="m-0"> Book a trip </span>
      </a>
    </nav>
  </div>
</header>
<main>
  {@render children()}
</main>
<footer>footer</footer>
