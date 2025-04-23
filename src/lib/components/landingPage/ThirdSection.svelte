<script lang="ts">
  interface Options {
    header: string;
    text: string;
    icon: string;
  }
  const discoverOptions: Options[] = [
    {
      header: "Handpicked Destinations",
      text: "Only the best locations, curated for unforgettable experiences",
      icon: '<i class="fa-solid fa-globe"></i>',
    },
    {
      header: "Seamless Booking",
      text: "Stress-free reservations with flexible options",
      icon: "<span>🧾</span>",
    },
    {
      header: "Expert Travel Guides",
      text: "Get personalized recommendations from industry pros",
      icon: "<span>📘</span>",
    },
    {
      header: "Hassle-Free Planning",
      text: "We handle the details, you enjoy the journey",
      icon: '<i class="fa-solid fa-circle-check"></i>',
    },
  ];
</script>

<section class=" px-6 py-16 text-center">
  <!-- Heading -->
  <h1 class="text-[2.45rem] mb-5 font-semibold">
    <div class="mb-2">Travel Smarter 🚀,</div>

    Explore Better 🌍
  </h1>

  <!-- Subheading -->
  <p class="text-gray-500 max-w-2xl mb-6 text-2xl mx-auto">
    Handpicked destinations, seamless bookings, and unbeatable
    experiences—because your journey deserves the best
  </p>

  <!-- CTA Button -->
  <div class="mb-12">
    <button
      class="bg-primary text-white px-12 py-4 rounded-full font-semibold hover:bg-blue-700 transition text-2xl light-font"
    >
      Discover <i class="fa-solid fa-circle-arrow-right"></i>
    </button>
  </div>

  <!-- Grid of Cards -->
  <div
    class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-6 max-w-4xl mx-auto"
  >
    <!-- Cards -->
    {#each discoverOptions as card}
      <div
        class="card text-white p-5
                rounded-2xl text-left w-sm h-60
                flex flex-row justify-center items-center"
      >
        <div class="m-auto">
          <div class="text-4xl mb-3">{@html card.icon}</div>
          <h3 class="text-3xl font-semibold mb-1 light-font">{card.header}</h3>
          <p class="text-md">
            {card.text}
          </p>
        </div>
      </div>
    {/each}
  </div>
</section>

<style>
  .card {
    background: linear-gradient(to bottom right, #1873cc, #003f7c);
  }
</style>
