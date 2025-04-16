<script lang="ts">
  let { headingStyle } = $props();
  let heading: string = "text-[20px] text-black ml-[-20px]";
  const listSpacing: string = "mb-[27px]";
</script>

<!-- Activities -->
<section class="text-left mx-auto">
  <h2 class={headingStyle}>Top Activities</h2>
  <div class="grid grid-cols-2 gap-2 text-[18px] text-gray-500 ml-[20px]">
    <ul class="space-y-1">
      <li class={listSpacing}>
        <span class={heading}>• Sunset Cruises</span> <br />Glide across golden
        skies over the Indian Ocean
      </li>
      <li class={listSpacing}>
        <span class={heading}>• Water Sports</span> <br />Try jet skiing,
        kayaking, or parasailing
      </li>
    </ul>
    <div class="place-items-end">
      <ul class="space-y-1">
        <li class={listSpacing}>
          <span class={heading}>• Underwater Diving</span> <br />Explore the
          depths beneath the sea of blue
        </li>
        <li class={listSpacing}>
          <span class={heading}>• Snorkeling & Diving</span> <br />Swim with
          manta rays and whale sharks
        </li>
      </ul>
    </div>
  </div>
</section>
