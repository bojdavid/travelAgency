<script lang="ts">
  interface navigation {
    nav: String;
    url: string;
  }
  let navs: navigation[] = [
    { nav: "Home", url: "/" },
    { nav: "Bookings", url: "/bookings" },
    { nav: "Contact Us", url: "/contact_us" },
    { nav: "Pricing", url: "/pricing" },
  ];
</script>

<div class="flex justify-center">
  <div class="w-[90px]">
    <p class="text-2xl mx-auto font-sofia font-weight-400">
      Soar <span class="inline-block transform rotate-320 ml-1">
        <i class="fa-solid fa-plane"></i>
      </span> Travels
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
