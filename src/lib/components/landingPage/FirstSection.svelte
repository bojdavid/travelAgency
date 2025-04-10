<script lang="ts">
  const images: number[] = [1, 2, 3, 4];
  const surroundImageStyle: string = "bg-stone-200 p-3 rounded-2xl";
  const textBelowFirstCTAstyles: string =
    "text-3xl text-gray-400 mt-1 font-light";
  const textBelowTextBelowFirstCTAstyles: string =
    "text-sm text-gray-400 mt-1 font-light";
</script>

<section class="py-16 text-center relative overflow-hidden">
  <!-- Floating Icons (emoji placeholders) -->
  <div
    class="absolute top-10 left-45 text-5xl rotate-25 {surroundImageStyle}  shadow-inner-lg"
  >
    🎢
  </div>
  <div class="absolute top-60 left-35 text-5xl {surroundImageStyle}">🏨</div>
  <div
    class="absolute top-105 left-45 text-5xl rotate-325 {surroundImageStyle}"
  >
    ⛱️
  </div>
  <!---  RIGHT ICONS -->
  <div
    class="absolute top-10 right-45 text-5xl rotate-325 {surroundImageStyle}"
  >
    🌍
  </div>
  <div class="absolute top-60 right-35 text-5xl {surroundImageStyle}">🔔</div>
  <div
    class="absolute top-105 right-45 text-5xl {surroundImageStyle} rotate-385"
  >
    🔔
  </div>

  <!-- Circle placeholders for images -->
  <div class="flex justify-center gap-8 mb-12">
    {#each images as image}
      <div
        class="w-[200px] h-[250px] rounded-full bg-gray-300 animate-pulse"
      ></div>
    {/each}
  </div>

  <!-- Headline -->
  <h1 class="text-6xl font-bold mb-10 mt-20">
    Plan. Book. <span class="text-blue-500">Travel. ✈️</span> Repeat.
  </h1>

  <!-- Subtext -->
  <p class="text-gray-500 text-2xl max-w-3xl mx-auto mb-10">
    Explore breathtaking destinations, hassle-free bookings and unbeatable deals
    - all at your fingertips.
  </p>

  <!-- CTA Buttons -->
  <div class="flex justify-center gap-6 mb-16 w-[480px] mx-auto">
    <button
      class="bg-blue-500 text-white px-8 py-4 rounded-full hover:bg-blue-600 transition w-[220px] text-2xl"
    >
      Book a trip →
    </button>
    <button
      class="bg-gray-100 px-8 py-4 rounded-full font-semibold text-gray-800 hover:bg-gray-200 transition w-[220px] text-2xl"
    >
      Watch demo
    </button>
  </div>

  <!-- Stats -->
  <div class="flex justify-center gap-32 text-center text-xl font-semibold">
    <div>
      <div class="text-5xl">
        100+ <i class="fa-solid fa-fire text-3xl my-auto"></i>
      </div>
      <p class={textBelowFirstCTAstyles}>Unique experiences</p>
      <p class={textBelowTextBelowFirstCTAstyles}>Handpicked by experts</p>
    </div>
    <div>
      <div class="text-5xl">30+ <i class="fa-solid fa-globe text-3xl"></i></div>
      <p class={textBelowFirstCTAstyles}>Destinations</p>
    </div>
    <div>
      <div class="text-5xl">
        2k+ <i class="fa-solid fa-user text-3xl my-auto"></i>
      </div>
      <p class={textBelowFirstCTAstyles}>Adventurers</p>
    </div>
  </div>
</section>
