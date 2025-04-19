<!-- ===================== HEADER ===================== -->
<header class="w-full border-b border-gray-100">
  <div class="mx-auto max-w-[1440px] px-6 py-6 flex justify-center">
    <form class="flex w-full max-w-3xl" action="#">
      <div class="relative flex-grow">
        <span
          class="absolute inset-y-0 left-0 flex items-center pl-3 text-gray-400"
        >
          <!-- search icon -->
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M8 16a8 8 0 1116 0 8 8 0 01-16 0z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M22 22l-4.35-4.35"
            />
          </svg>
        </span>
        <input
          type="text"
          placeholder="Search destination"
          class="w-full rounded-l-full border border-gray-300 bg-gray-50 py-3 pl-11 pr-4 text-sm focus:border-blue-500 focus:ring-2 focus:ring-blue-500"
        />
      </div>
      <button
        type="submit"
        class="rounded-r-full bg-blue-600 px-8 text-sm font-medium text-white transition hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500"
      >
        Search
      </button>
    </form>
  </div>
</header>

<!-- ===================== FILTER TABS ===================== -->
<nav class="mx-auto max-w-[1440px] px-6 mt-10">
  <ul class="flex flex-wrap gap-6 text-sm font-medium text-gray-500">
    <li><a href="#" class="hover:text-blue-600">All Destinations</a></li>
    <li><a href="#" class="hover:text-blue-600">Most Popular</a></li>
    <li>
      <a href="#" class="border-b-2 border-blue-600 pb-1 text-blue-600"
        >Beaches</a
      >
    </li>
    <li><a href="#" class="hover:text-blue-600">Cities</a></li>
    <li><a href="#" class="hover:text-blue-600">Nightlife</a></li>
    <li><a href="#" class="hover:text-blue-600">Mountains</a></li>
  </ul>
</nav>

<!-- ===================== DESTINATION GRID ===================== -->
<section
  class="mx-auto max-w-[1440px] px-6 mt-12 grid gap-12 sm:grid-cols-2 lg:grid-cols-3"
>
  <!-- CARD TEMPLATE (copy‑paste for each destination) -->
  <article class="space-y-4">
    <!-- Placeholder image -->
    <div class="h-56 w-full rounded-2xl bg-gray-200 animate-pulse"></div>

    <div class="flex items-center justify-between">
      <h3 class="text-lg font-semibold">Maldives</h3>
      <a
        href="#"
        class="group flex items-center gap-1 text-blue-600 hover:underline"
      >
        View
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4 transition-transform group-hover:translate-x-1"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M5 12h14M12 5l7 7-7 7"
          />
        </svg>
      </a>
    </div>

    <p class="text-xs text-gray-500">
      Category • <span class="font-medium text-gray-800">Luxury • Beach</span>
    </p>

    <div class="flex items-center gap-1 text-xs text-gray-500">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-4 w-4 text-yellow-400"
        viewBox="0 0 20 20"
        fill="currentColor"
      >
        <path
          d="M9.049 2.927C9.34 2.054 10.66 2.054 10.951 2.927l1.073 3.302a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.073 3.302c.292.873-.755 1.598-1.538 1.028l-2.8-2.034a1 1 0 00-1.176 0l-2.8 2.034c-.783.57-1.83-.155-1.538-1.028l1.073-3.302a1 1 0 00-.364-1.118L2.453 8.73c-.783-.57-.38-1.81.588-1.81h3.462a1 1 0 00.95-.69l1.073-3.302z"
        />
      </svg>
      4.5
    </div>

    <p class="text-xs text-gray-500">
      Pricing<br />
      <span class="text-base font-semibold text-gray-800">From $1200</span>
      <span class="text-gray-400"> / Person</span>
    </p>
  </article>

  <!-- CARD CLONE -->
  <article class="space-y-4">
    <div class="h-56 w-full rounded-2xl bg-gray-200 animate-pulse"></div>
    <div class="flex items-center justify-between">
      <h3 class="text-lg font-semibold">Bahamas</h3>
      <a
        href="#"
        class="group flex items-center gap-1 text-blue-600 hover:underline"
      >
        View
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4 transition-transform group-hover:translate-x-1"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M5 12h14M12 5l7 7-7 7"
          />
        </svg>
      </a>
    </div>
    <p class="text-xs text-gray-500">
      Category • <span class="font-medium text-gray-800">Luxury • Beach</span>
    </p>
    <div class="flex items-center gap-1 text-xs text-gray-500">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-4 w-4 text-yellow-400"
        viewBox="0 0 20 20"
        fill="currentColor"
      >
        <path
          d="M9.049 2.927C9.34 2.054 10.66 2.054 10.951 2.927l1.073 3.302a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.073 3.302c.292.873-.755 1.598-1.538 1.028l-2.8-2.034a1 1 0 00-1.176 0l-2.8-2.034c-.783.57-1.83-.155-1.538-1.028l1.073-3.302a1 1 0 00-.364-1.118L2.453 8.73c-.783-.57-.38-1.81.588-1.81h3.462a1 1 0 00.95-.69l1.073-3.302z"
        />
      </svg>
      4.6
    </div>
    <p class="text-xs text-gray-500">
      Pricing<br />
      <span class="text-base font-semibold text-gray-800">From $1800</span>
      <span class="text-gray-400"> / Person</span>
    </p>
  </article>

  <!-- CARD CLONE -->
  <article class="space-y-4">
    <div class="h-56 w-full rounded-2xl bg-gray-200 animate-pulse"></div>
    <div class="flex items-center justify-between">
      <h3 class="text-lg font-semibold">Barbados</h3>
      <a
        href="#"
        class="group flex items-center gap-1 text-blue-600 hover:underline"
      >
        View
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4 transition-transform group-hover:translate-x-1"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M5 12h14M12 5l7 7-7 7"
          />
        </svg>
      </a>
    </div>
    <p class="text-xs text-gray-500">
      Category • <span class="font-medium text-gray-800">Luxury • Beach</span>
    </p>
    <div class="flex items-center gap-1 text-xs text-gray-500">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="h-4 w-4 text-yellow-400"
        viewBox="0 0 20 20"
        fill="currentColor"
      >
        <path
          d="M9.049 2.927C9.34 2.054 10.66 2.054 10.951 2.927l1.073 3.302a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.073 3.302c.292.873-.755 1.598-1.538 1.028l-2.8-2.034a1 1 0 00-1.176 0l-2.8-2.034c-.783.57-1.83-.155-1.538-1.028l1.073-3.302a1 1 0 00-.364-1.118L2.453 8.73c-.783-.57-.38-1.81.588-1.81h3.462a1 1 0 00.95-.69l1.073-3.302z"
        />
      </svg>
      4.2
    </div>
    <p class="text-xs text-gray-500">
      Pricing<br />
      <span class="text-base font-semibold text-gray-800">From $1200</span>
      <span class="text-gray-400"> / Person</span>
    </p>
  </article>

  <!-- Repeat above article blocks as needed to fill the grid -->
</section>
