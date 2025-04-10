<script lang="ts">
  import "../lib/styles/app.css";

  import FirstSection from "$lib/components/landingPage/FirstSection.svelte";
  import SecondSection from "$lib/components/landingPage/SecondSection.svelte";
  import ThirdSection from "$lib/components/landingPage/ThirdSection.svelte";
  import FourthSection from "$lib/components/landingPage/FourthSection.svelte";
  import FifthSection from "$lib/components/landingPage/FifthSection.svelte";
</script>

<div class="flex flex-col justify-center items-center">
  <FirstSection />
  <SecondSection />
  <ThirdSection />
  <FourthSection />
  <FifthSection />
</div>
