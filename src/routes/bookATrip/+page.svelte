<section class="bg-white font-sans text-gray-800">
  <main class="w-[1440px] mx-auto px-12 py-10 space-y-12">
    <!-- Search Bar -->
    <div class="flex justify-center gap-4">
      <div class="relative w-[600px]">
        <input
          type="text"
          placeholder="Search destination"
          class="w-full border border-gray-300 rounded-full px-12 py-3 text-sm shadow-sm outline-none focus:ring-2 focus:ring-blue-400"
        />
        <span class="absolute left-4 top-3.5 text-gray-400 text-lg">🔍</span>
      </div>
      <button
        class="bg-blue-600 text-white px-8 py-3 rounded-full hover:bg-blue-700 transition"
      >
        Search
      </button>
    </div>

    <!-- Category Filters -->
    <div class="flex justify-center gap-10 font-medium text-sm text-gray-700">
      <button class="text-blue-600 border-b-2 border-blue-600 pb-1"
        >All Destinations</button
      >
      <button class="hover:text-blue-600">Most Popular</button>
      <button class="hover:text-blue-600">Beaches</button>
      <button class="hover:text-blue-600">Cities</button>
      <button class="hover:text-blue-600">Nightlife</button>
      <button class="hover:text-blue-600">Mountains</button>
    </div>

    <!-- Destination Grid -->
    <div class="grid grid-cols-3 gap-x-10 gap-y-12">
      <!-- Destination Card Template (reusable) -->
      <div class="space-y-3">
        <div class="w-full h-[180px] rounded-xl bg-gray-200 overflow-hidden">
          <img
            src="https://via.placeholder.com/300x180"
            alt="Maldives"
            class="w-full h-full object-cover"
          />
        </div>
        <div class="flex justify-between items-center">
          <h3 class="font-semibold text-lg">Maldives</h3>
          <a href="#" class="text-blue-500 text-sm flex items-center gap-1"
            >View →</a
          >
        </div>
        <div class="text-sm text-gray-600 space-y-1">
          <p>
            <span class="font-semibold text-gray-800">Category:</span> Luxury • Beach
          </p>
          <p><span class="font-semibold text-gray-800">Rating:</span> ⭐ 4.5</p>
          <p>
            <span class="font-semibold text-gray-800">Pricing:</span> From $1200
            / Person
          </p>
        </div>
      </div>

      <!-- Copy or loop this card structure for other locations -->
      <div class="space-y-3">
        <div class="w-full h-[180px] rounded-xl bg-gray-200 overflow-hidden">
          <img
            src="https://via.placeholder.com/300x180"
            alt="Bahamas"
            class="w-full h-full object-cover"
          />
        </div>
        <div class="flex justify-between items-center">
          <h3 class="font-semibold text-lg">Bahamas</h3>
          <a href="#" class="text-blue-500 text-sm flex items-center gap-1"
            >View →</a
          >
        </div>
        <div class="text-sm text-gray-600 space-y-1">
          <p>
            <span class="font-semibold text-gray-800">Category:</span> Luxury • Beach
          </p>
          <p><span class="font-semibold text-gray-800">Rating:</span> ⭐ 4.6</p>
          <p>
            <span class="font-semibold text-gray-800">Pricing:</span> From $1800
            / Person
          </p>
        </div>
      </div>

      <!-- Another card -->
      <div class="space-y-3">
        <div class="w-full h-[180px] rounded-xl bg-gray-200 overflow-hidden">
          <img
            src="https://via.placeholder.com/300x180"
            alt="Barbados"
            class="w-full h-full object-cover"
          />
        </div>
        <div class="flex justify-between items-center">
          <h3 class="font-semibold text-lg">Barbados</h3>
          <a href="#" class="text-blue-500 text-sm flex items-center gap-1"
            >View →</a
          >
        </div>
        <div class="text-sm text-gray-600 space-y-1">
          <p>
            <span class="font-semibold text-gray-800">Category:</span> Luxury • Beach
          </p>
          <p><span class="font-semibold text-gray-800">Rating:</span> ⭐ 4.2</p>
          <p>
            <span class="font-semibold text-gray-800">Pricing:</span> From $1200
            / Person
          </p>
        </div>
      </div>

      <!-- Repeat the 3-card pattern again for the second row -->
      <!-- In production, you'd likely loop through these with dynamic data -->
    </div>
  </main>
</section>
