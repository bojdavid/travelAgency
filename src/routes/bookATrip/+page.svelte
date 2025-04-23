<script lang="ts">
  import DestinationCard from "$lib/components/bookAtrip/DestinationCard.svelte";
  import NewsLetter from "$lib/components/NewsLetter.svelte";

  const filter: string[] = [
    "All Destinations",
    "Most Popular",
    "Beaches",
    "Cities",
    "Nightlife",
    "Mountains",
  ];

  interface Destination {
    name: string;
    category: string[];
    rating: number;
    pricing: number;
  }

  const destinationList: Destination[] = [
    { name: "Taj Mahal", category: ["Landmark"], rating: 4.0, pricing: 53 },
    {
      name: "Taj Mahal",
      category: ["Nature", "Shopping"],
      rating: 4.3,
      pricing: 82,
    },
    {
      name: "Great Barrier Reef",
      category: ["Landmark", "Historical", "Shopping"],
      rating: 4.2,
      pricing: 93,
    },
    {
      name: "Niagara Falls",
      category: ["Cultural", "Urban"],
      rating: 4.7,
      pricing: 83,
    },
    {
      name: "Stonehenge",
      category: ["Historical", "Cultural"],
      rating: 4.7,
      pricing: 91,
    },
    {
      name: "Grand Canyon",
      category: ["Nature", "Shopping"],
      rating: 3.6,
      pricing: 55,
    },
    {
      name: "Machu Picchu",
      category: ["Historical", "Nature", "Urban"],
      rating: 4.6,
      pricing: 51,
    },
    {
      name: "Statue of Liberty",
      category: ["Nature"],
      rating: 4.6,
      pricing: 39,
    },
    {
      name: "Eiffel Tower",
      category: ["Urban", "Shopping"],
      rating: 3.9,
      pricing: 17,
    },
    { name: "Stonehenge", category: ["Landmark"], rating: 4.7, pricing: 35 },
    {
      name: "Central Park",
      category: ["Nature", "Entertainment"],
      rating: 4.4,
      pricing: 13,
    },
    { name: "Mount Everest", category: ["Cultural"], rating: 4.7, pricing: 83 },
    {
      name: "Santorini",
      category: ["Adventure", "Landmark"],
      rating: 4.4,
      pricing: 77,
    },
    {
      name: "Great Barrier Reef",
      category: ["Urban", "Adventure", "Entertainment"],
      rating: 3.7,
      pricing: 16,
    },
    { name: "Taj Mahal", category: ["Adventure"], rating: 4.8, pricing: 65 },
    {
      name: "Mount Everest",
      category: ["Entertainment", "Adventure"],
      rating: 4.0,
      pricing: 51,
    },
    { name: "Santorini", category: ["Shopping"], rating: 4.2, pricing: 99 },
    {
      name: "Grand Canyon",
      category: ["Shopping", "Adventure", "Nature"],
      rating: 4.5,
      pricing: 48,
    },
    { name: "Petra", category: ["Nature"], rating: 3.6, pricing: 12 },
    { name: "Niagara Falls", category: ["Landmark"], rating: 4.0, pricing: 89 },
    {
      name: "Times Square",
      category: ["Adventure", "Shopping"],
      rating: 4.1,
      pricing: 31,
    },
    {
      name: "Angkor Wat",
      category: ["Shopping", "Cultural", "Landmark"],
      rating: 4.7,
      pricing: 59,
    },
    { name: "Chichen Itza", category: ["Landmark"], rating: 5.0, pricing: 57 },
    {
      name: "Angkor Wat",
      category: ["Urban", "Shopping", "Historical"],
      rating: 3.9,
      pricing: 40,
    },
    {
      name: "Mount Everest",
      category: ["Shopping", "Urban"],
      rating: 4.5,
      pricing: 92,
    },
    {
      name: "Niagara Falls",
      category: ["Urban", "Historical"],
      rating: 4.8,
      pricing: 37,
    },
    { name: "Santorini", category: ["Shopping"], rating: 3.6, pricing: 64 },
    {
      name: "Colosseum",
      category: ["Urban", "Shopping", "Nature"],
      rating: 4.1,
      pricing: 73,
    },
    {
      name: "Machu Picchu",
      category: ["Landmark", "Cultural", "Nature"],
      rating: 4.1,
      pricing: 46,
    },
    {
      name: "Great Barrier Reef",
      category: ["Cultural", "Shopping", "Urban"],
      rating: 4.1,
      pricing: 45,
    },
  ];
  let active: string = $state("All Destinations");
  const selectActive = (item: string) => {
    active = item;
  };
  const activeStyle: string =
    "border-b-2 border-blue-600 pb-1 text-blue-500 transition duration-200 ease-in-out";
</script>

<!-- ===================== HEADER ===================== -->
<header class="w-full my-20">
  <div class="mx-auto px-6 py-6 flex justify-center">
    <form class="flex gap-5" action="#">
      <div class="relative flex w-[520px] rounded-full">
        <span
          class="absolute inset-y-0 left-4 flex items-center pl-3 text-gray-400"
        >
          <!-- search icon -->
          <svg
            fill="#ACACAC"
            height="20px"
            width="20px"
            version="1.1"
            id="Capa_1"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            viewBox="0 0 488.4 488.4"
            xml:space="preserve"
            ><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
              id="SVGRepo_tracerCarrier"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></g><g id="SVGRepo_iconCarrier">
              <g>
                <g>
                  <path
                    d="M0,203.25c0,112.1,91.2,203.2,203.2,203.2c51.6,0,98.8-19.4,134.7-51.2l129.5,129.5c2.4,2.4,5.5,3.6,8.7,3.6 s6.3-1.2,8.7-3.6c4.8-4.8,4.8-12.5,0-17.3l-129.6-129.5c31.8-35.9,51.2-83,51.2-134.7c0-112.1-91.2-203.2-203.2-203.2 S0,91.15,0,203.25z M381.9,203.25c0,98.5-80.2,178.7-178.7,178.7s-178.7-80.2-178.7-178.7s80.2-178.7,178.7-178.7 S381.9,104.65,381.9,203.25z"
                  ></path>
                </g>
              </g>
            </g></svg
          >
        </span>
        <input
          type="text"
          placeholder="Search destination"
          class="w-full h-[64px] rounded-full border border-gray-200 bg-gray-50 py-3 pl-15 pr-4 text-[18px] focus:border-blue-500 focus:ring-2 focus:ring-blue-500"
        />
      </div>
      <button
        type="submit"
        class="rounded-full bg-blue-600 px-8 text-[24px] w-[170px] h-[64px] text-white transition hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500"
      >
        Search
      </button>
    </form>
  </div>
</header>

<main class="w-[980px] mx-auto">
  <!-- ===================== FILTER TABS ===================== -->
  <nav class="my-10">
    <ul
      class="flex flex-wrap gap-[40px] text-sm font-medium text-gray-900 text-[18px]"
    >
      {#each filter as place}
        <li>
          <button
            class="hover:text-blue-600 {active == place ? activeStyle : ''}"
            onclick={() => selectActive(place)}>{place}</button
          >
        </li>
      {/each}
    </ul>
  </nav>

  <section class="flex flex-wrap justify-center gap-10">
    <!-- ===================== DESTINATION GRID ===================== -->
    {#each destinationList as destination}
      <DestinationCard {destination} />
    {/each}
  </section>

  <section class="mb-30">
    <NewsLetter />
  </section>
</main>
