<script lang="ts">
  const company: any = [
    { link: "#", name: "About Us" },
    { link: "#", name: "Contact Us" },
    { link: "#", name: "Testimonials" },
    { link: "#", name: "Career" },
  ];

  const travel: any = [
    { link: "#", name: "Flights" },
    { link: "#", name: "Destinations" },
    { link: "#", name: "Hotels" },
    { link: "#", name: "Vacation Packages" },
    { link: "#", name: "FAQ" },
  ];

  const legal: any = [
    { link: "#", name: "Terms & Conditions" },
    { link: "#", name: "Privacy Policy" },
    { link: "#", name: "Cookie Policy" },
  ];
</script>

<div class="bg-blue-600 text-white rounded-4xl px-9 py-10 font-hanken">
  <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-4 gap-8">
    <!-- Logo -->
    <div class="w-[100px]">
      <h2 class="text-2xl font-logo mb-4 font-sofia">
        Soar<span class="inline-block transform rotate-320 ml-1">
          <i class="fa-solid fa-plane"></i>
        </span>Travels
      </h2>
    </div>

    <!-- Company -->
    <div>
      <h3 class="font-semibold mb-3 text-2xl">Company</h3>
      <ul class="space-y-2 text-md">
        {#each company as c}
          <li><a href={c.link} class="hover:underline">{c.name}</a></li>
        {/each}
      </ul>
    </div>

    <!-- Travel -->
    <div>
      <h3 class="font-semibold mb-3 text-2xl">Travel</h3>
      <ul class="space-y-2 text-md">
        {#each travel as c}
          <li><a href={c.link} class="hover:underline">{c.name}</a></li>
        {/each}
      </ul>
    </div>

    <!-- Legal -->
    <div>
      <h3 class="font-semibold mb-3 text-2xl">Legal</h3>
      <ul class="space-y-2 text-md">
        {#each legal as c}
          <li><a href={c.link} class="hover:underline">{c.name}</a></li>
        {/each}
      </ul>
    </div>
  </div>

  <!-- Bottom bar -->
  <div
    class="mt-10 border-t border-white/30 pt-6 flex flex-col md:flex-row justify-between items-center text-md"
  >
    <div class="flex space-x-4 mb-4 md:mb-0">
      <a href="#"><i class="fab fa-x-twitter"></i></a>
      <a href="#"><i class="fab fa-instagram"></i></a>
      <a href="#"><i class="fab fa-youtube"></i></a>
      <a href="#"><i class="fab fa-facebook"></i></a>
    </div>
    <div class="space-x-4">
      <a href="#" class="hover:underline">Terms of Service</a>
      <a href="#" class="hover:underline">Privacy Policy</a>
    </div>
  </div>
</div>
