<script lang="ts">
  const lineStyle: string =
    "h-1 w-full bg-gradient-to-r from-transparent via-gray-300 to-transparent my-auto";

  interface CardData {
    id: number;
    category: string;
    rating: number;
    pricing: number;
  }
  const cards: CardData[] = [
    { id: 1, category: "Web Development", rating: 4.8, pricing: 299 },
    { id: 2, category: "Graphic Design", rating: 4.5, pricing: 199 },
    { id: 3, category: "Data Science", rating: 4.9, pricing: 349 },
    { id: 4, category: "Digital Marketing", rating: 4.4, pricing: 179 },
    { id: 5, category: "Photography", rating: 4.6, pricing: 149 },
    { id: 6, category: "UI/UX Design", rating: 4.7, pricing: 269 },
    { id: 7, category: "Finance & Accounting", rating: 4.3, pricing: 159 },
    { id: 8, category: "Mobile App Development", rating: 4.8, pricing: 329 },
    { id: 9, category: "Cybersecurity", rating: 4.9, pricing: 379 },
    { id: 10, category: "Game Development", rating: 4.6, pricing: 289 },
  ];
</script>

<!-- Title -->
<h1
  class="text-3xl font-light italic text-primary pb-1 font-satisfy flex flex-row"
>
  <div class={lineStyle}></div>

  Maldives

  <div class={lineStyle}></div>
</h1>

<!-- Main Image Placeholder -->
<div class="flex justify-center">
  <div class="w-[857px] h-[300px] rounded-4xl bg-gray-200 animate-pulse"></div>
</div>

<!-- Image Gallery -->
<div class="flex justify-center items-center gap-4 mt-4">
  <button class="text-2xl">&larr;</button>
  <div class="flex gap-2">
    <div
      class="w-20 h-16 bg-gray-200 rounded-md animate-pulse border-2 border-blue-500"
    ></div>
    <div class="w-20 h-16 bg-gray-200 rounded-md animate-pulse"></div>
    <div class="w-20 h-16 bg-gray-200 rounded-md animate-pulse"></div>
  </div>
  <button class="text-2xl">&rarr;</button>
</div>

<!-- Info Tags -->
<div class="flex justify-center gap-8 text-sm">
  <p><span class="font-semibold">Category:</span> Luxury • Beach</p>
  <p><span class="font-semibold">Rating:</span> ⭐ 4.6</p>
  <p><span class="font-semibold">Pricing:</span> From $1800 / person</p>
</div>
