<script lang="ts">
  import { slide } from "svelte/transition";

  let { questions } = $props();

  const toggleViewText = (viewText: boolean, index: number) => {
    questions[index].viewText = !viewText;
  };
</script>

<section class="mx-auto px-6 text-center">
  <!-- FAQ Accordion -->
  <div class="w-4xl mx-auto space-y-4 text-left">
    {#each questions as question, index (question)}
      <div class="border-b border-gray-200 pb-4">
        <button
          class="flex justify-between items-center cursor-pointer w-full"
          onclick={() => toggleViewText(question.viewText, index)}
        >
          <h3 class="text-2xl">
            {question.question}
          </h3>
          <span
            class="text-2xl transform transition duration-500 ease-in-out {question.viewText
              ? ''
              : 'rotate-180'}"
            aria-label="angle_up"><i class="fa-solid fa-angle-up"></i></span
          >
        </button>
        {#if question.viewText}
          <div class="overflow-hidden" transition:slide={{ duration: 500 }}>
            <p class="mt-2 text-gray-500 text-lg light-font">
              {question.answer}
            </p>
          </div>
        {/if}
      </div>
    {/each}
  </div>
</section>
