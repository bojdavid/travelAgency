<script lang="ts">
  let { headingStyle } = $props();
  const heading: string = "";
  const listSpacing: string = "mb-[20px]";
</script>

<!-- Where to Stay -->
<section class="text-left mx-auto">
  <h2 class={headingStyle}>Where to Stay</h2>
  <div class="grid grid-cols-3 gap-6 text-[18px] ml-[20px]">
    <div class="">
      <h3 class="font-semibold {listSpacing} bullet">Luxury</h3>
      <ul class="text-primary">
        <li class={listSpacing}>The St. Regis Maldives</li>
        <li class={listSpacing}>Baros Maldives</li>
      </ul>
    </div>
    <div>
      <h3 class="font-semibold {listSpacing} bullet">Mid Range</h3>
      <ul class="text-primary">
        <li class={listSpacing}>Reethi Beach Resort</li>
        <li class={listSpacing}>Kurumba Resort & Spa</li>
        <li class={listSpacing}>Meeru Island Resort</li>
      </ul>
    </div>
    <div>
      <h3 class="font-semibold {listSpacing} bullet">Budget Friendly</h3>
      <ul class="text-primary">
        <li class={listSpacing}>Maafushi Dive Lodge</li>
        <li class={listSpacing}>Kaani Palm Beach</li>
      </ul>
    </div>
  </div>
</section>

<style>
  .bullet {
    display: list-item;
    list-style-type: disc;
  }
</style>
