<script lang="ts">
  let { place, description, category, rating, price } = $props();
</script>

<div
  class="relative z-10 bg-white rounded-4xl overflow-hidden shadow-lg border-10 border-gray-100"
>
  <!-- Image Placeholder -->
  <div class="h-64 rounded-lg bg-gray-300 animate-pulse m-5"></div>

  <!-- Card Content -->
  <div class="px-5 text-lg">
    <h2 class="text-4xl font-semibold mb-2">{place}</h2>
    <p class="text-gray-500 mb-4 text-lg light-font w-md">
      {description}
    </p>

    <div class="flex justify-evenly text-sm mb-4 gap-6">
      <div class="flex self-end">
        <div class="text-lg w-40">
          <p class="text-gray-400 text-lg light-font">Category</p>
          <p>
            <span class="font-semibold">{category}</span> •
          </p>
        </div>

        <div class="text-xl mr-7">
          <p class="text-gray-400 text-lg light-font">Rating</p>
          <p>⭐ {rating.rating}</p>
        </div>
        <div class="text-xl">
          <p class="text-gray-400 text-lg light-font">Pricing</p>
          <p class="text-gray-400">
            <span class="text-black">From</span>
            <span class="font-semibold text-black">${price}</span> / Person
          </p>
        </div>
      </div>

      <!-- Buttons -->
      <div class="flex flex-col justify-end gap-4">
        <button
          class="px-3 py-3 rounded-full border border-gray-300 text-2xl hover:bg-gray-100 transition text-gray-500"
        >
          See details <i class="fa-solid fa-circle-right"></i>
        </button>
        <button
          class="px-3 py-3 rounded-full bg-blue-600 text-white text-2xl hover:bg-blue-700 transition"
        >
          Book now <i class="fa-solid fa-circle-right"></i>
        </button>
      </div>
    </div>
  </div>
</div>
