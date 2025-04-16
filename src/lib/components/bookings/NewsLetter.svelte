<script lang="ts">
  let { headingStyle } = $props();
</script>

<section class=" py-10 mt-12 rounded-md mx-auto w-[527px]">
  <h2 class="text-[28px] font-semibold mb-[15px]">
    Be the First to Discover New Destinations
  </h2>
  <p class="text-[18px] text-gray-500 mb-4 w-[445px] mx-auto">
    Subscribe to get the latest travel deals, destination guides, and exclusive
    offers straight to your inbox.
  </p>
  <div class="flex flex-col justify-center gap-[50px] mt-14 items-center">
    <input
      type="email"
      placeholder="Enter your email address"
      class="border border-gray-300 px-4 text-[16px] py-2 rounded-2xl w-full mx-[10px] h-[60px] placeholder-gray-300"
    />
    <button
      class="bg-blue-600 w-[300px] text-[24px] h-[64px] text-white px-6 py-2 rounded-full hover:bg-blue-700 transition"
      >Subscribe</button
    >
  </div>
</section>
