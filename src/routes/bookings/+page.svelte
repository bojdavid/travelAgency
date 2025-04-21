<script lang="ts">
  import Card from "$lib/components/bookings/Card.svelte";
  import TopActivities from "$lib/components/bookings/TopActivities.svelte";
  import WhereToStay from "$lib/components/bookings/whereToStay.svelte";
  import NewsLetter from "$lib/components/NewsLetter.svelte";

  const headingStyle: string = "text-[24px] font-[500] text-blue-700 mb-2";
  const whereToStayListHeading = "text-[20px] font-[500] leading-[27px]";
  const marginBottom: string = "mb-[8em]";

  const topActivitiesContent = [
    {
      topic: "Sunset Cruises",
      content: "Glide across golden skies over the Indian Ocean",
    },
    {
      topic: "Water Sports",
      content: "Try jet skiing, kayaking, or parasailing",
    },
    {
      topic: "Underwater Diving",
      content: " Explore the depths beneath the sea of blue ",
    },
    { topic: "", content: "" },
    {
      topic: "Snorkeling & Diving<",
      content: "Swim with manta rays and whale sharks",
    },
  ];
</script>

<section class="bg-white font-sans text-gray-800">
  <main class="w-[883px] mx-auto px-6 py-10 space-y-12 text-center">
    <Card />

    <!-- Button -->
    <button
      class="bg-blue-600 text-white px-6 py-2 rounded-full hover:bg-blue-700 transition w-[500px] p-[10px] h-[64px] text-[24px]"
      >Book trip</button
    >

    <!-- Overview Section -->
    <section class="text-left mx-auto {marginBottom}">
      <h2 class={headingStyle}>Overview</h2>
      <p class="text-[18px] leading-[24px]">
        Crystal-clear turquoise waters, powdery white sands, and luxurious
        overwater bungalows—welcome to the Maldives. Whether you’re seeking a
        tranquil escape or an ocean-fronted adventure, breathtaking marine life,
        and unmatched serenity are just some of the world’s most stunning island
        destinations.
      </p>
    </section>
    <div class={marginBottom}>
      <TopActivities {headingStyle} />
    </div>
    <div class={marginBottom}>
      <WhereToStay {headingStyle} />
    </div>
    <div class={marginBottom}>
      <!-- Newsletter -->
      <NewsLetter />
    </div>
  </main>
</section>
