<script lang="ts">
  let { destination } = $props();
  const titleStyle: string = "text-[12px]";

  interface Destination {
    name: string;
    category: string[];
    rating: number;
    pricing: number;
  }
</script>

<!-- CARD TEMPLATE (copy‑paste for each destination) -->
<article class="space-y-4">
  <!-- Placeholder image -->
  <div class="h-[180px] w-[300px] rounded-2xl bg-gray-200 animate-pulse"></div>

  <div class="flex items-center justify-between">
    <h3 class="text-[20px] font-[500]">{destination.name}</h3>
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

  <div class="flex justify-between">
    <div class="text-xs text-gray-500 w-[102px]">
      <h5 class={titleStyle}>Category</h5>
      <p class="font-medium text-gray-800 text-[14px] flex">
        {#each destination.category as category}
          {category} •
        {/each}
      </p>
    </div>

    <div class="text-[14px] text-gray-500">
      <h5 class={titleStyle}>Rating</h5>
      <div class="flex">
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
        {destination.rating}
      </div>
    </div>

    <div class="text-[12px] text-gray-500">
      <h5 class={titleStyle}>Pricing</h5>
      <p>
        From
        <span class="text-base font-[400] text-gray-800 text-[14px]">
          ${destination.pricing}</span
        ><br />
        /Person
      </p>
    </div>
  </div>
</article>
