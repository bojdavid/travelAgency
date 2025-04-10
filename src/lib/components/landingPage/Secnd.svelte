<script lang="ts">
  import CardSecond from "./CardSecond.svelte";
  let card;

  interface CardData {
    place: string;
    description: string;
    category: string;
    rating: { star: string; rating: number };
    price: number;
  }

  const cardDataList: CardData[] = [
    {
      place: "Paris, France",
      description:
        "A romantic hub known for its art, cuisine, and timeless charm.",
      category: "Romantic & Cultural",
      rating: { star: "⭐", rating: 4.8 },
      price: 220,
    },
    {
      place: "New York City, USA",
      description:
        "The bustling metropolis famous for its iconic skyline and diverse culture.",
      category: "Urban Adventure",
      rating: { star: "⭐", rating: 4.5 },
      price: 300,
    },
    {
      place: "Tokyo, Japan",
      description:
        "A vibrant city where futuristic technology meets traditional charm.",
      category: "Cultural & Modern",
      rating: { star: "⭐", rating: 4.7 },
      price: 280,
    },
    {
      place: "Rome, Italy",
      description:
        "Historic streets filled with ancient ruins and world-class cuisine.",
      category: "Historical & Cultural",
      rating: { star: "⭐", rating: 4.6 },
      price: 200,
    },
    {
      place: "Sydney, Australia",
      description:
        "An iconic city known for its harbor, beaches, and lively arts scene.",
      category: "Beach & Urban",
      rating: { star: "⭐", rating: 4.7 },
      price: 250,
    },
    {
      place: "Cape Town, South Africa",
      description:
        "A stunning destination with dramatic landscapes and rich diversity.",
      category: "Adventure & Nature",
      rating: { star: "⭐", rating: 4.5 },
      price: 180,
    },
    {
      place: "Barcelona, Spain",
      description:
        "A vibrant city famous for Gaudí's architecture and Mediterranean flair.",
      category: "Cultural & Modern",
      rating: { star: "⭐", rating: 4.6 },
      price: 210,
    },
    {
      place: "Dubai, UAE",
      description:
        "A luxurious, futuristic city with record-breaking skyscrapers and shopping.",
      category: "Luxury & Urban",
      rating: { star: "⭐", rating: 4.8 },
      price: 350,
    },
    {
      place: "Amsterdam, Netherlands",
      description:
        "Charming canals, museums, and a laid-back vibe in a historic setting.",
      category: "Cultural & Scenic",
      rating: { star: "⭐", rating: 4.7 },
      price: 230,
    },
    {
      place: "Bali, Indonesia",
      description:
        "A tropical paradise known for its beaches, temples, and vibrant culture.",
      category: "Relaxation & Adventure",
      rating: { star: "⭐", rating: 4.6 },
      price: 190,
    },
  ];
  let cardNumber: number = $state(0);
</script>

<section>
  <div class="text-center w-xl">
    <h1 class="text-5xl font-semibold mb-5 mt-15">Top Destinations</h1>
    <p class="text-2xl text-gray-400">
      Explore breath taking destinations, hassle-free booking and unbeatable
      deals - all at your finger tips
    </p>
  </div>

  <!-- CTA Button -->
  <div class="my-12 flex justify-center">
    <button
      class="bg-blue-600 text-white px-12 py-4 rounded-full font-semibold hover:bg-blue-700 transition text-2xl light-font"
    >
      Discover <i class="fa-solid fa-circle-arrow-right"></i>
    </button>
  </div>
</section>

<section class="w-5xl mx-auto py-16 flex items-center justify-center relative">
  <!-- Left Arrow -->
  <button
    aria-label="prev"
    class="absolute left-5 bg-gray-100 hover:bg-gray-200 p-4 rounded-full text-xl shadow"
  >
    <i class="fa-solid fa-circle-left"></i>
  </button>

  <!-- Card Stack -->
  <div class="relative w-[750px] max-w-full">
    <!-- Background Cards (simulate stack) -->
    <div
      class="absolute inset-0 translate-x-5 rotate-8 bg-gray-500 rounded-4xl border border-gray-200 z-1"
    ></div>
    <div
      class="absolute inset-0 -translate-x -translate-y-5 -rotate-7 bg-gray-900 rounded-4xl border border-gray-200 z-0"
    ></div>
    <div
      class="absolute inset-0 translate-x -rotate-3 bg-gray-300 rounded-4xl border border-gray-200 z-1"
    ></div>

    <!-- Main Card -->
    <CardSecond
      place={cardDataList[cardNumber].place}
      description={cardDataList[cardNumber].description}
      category={cardDataList[cardNumber].category}
      price={cardDataList[cardNumber].price}
      rating={cardDataList[cardNumber].rating}
    />
  </div>

  <!-- Right Arrow -->
  <button
    aria-label="next"
    class="absolute right-5 bg-gray-100 hover:bg-gray-200 p-4 rounded-full text-xl shadow"
  >
    <i class="fa-solid fa-circle-right"></i>
  </button>
</section>
