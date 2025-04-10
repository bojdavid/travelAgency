<script lang="ts">
  import { slide } from "svelte/transition";

  interface Question {
    question: string;
    answer: string;
    viewText: boolean;
  }

  const toggleViewText = (viewText: boolean, index: number) => {
    questions[index].viewText = !viewText;
  };

  let questions: Question[] = $state([
    {
      question: "How do I book a trip with Soar Travel?",
      answer:
        "Booking with Soar Travel is easy! Simply browse our destinations, select your preferred flights and accommodations, and proceed to checkout. You can customize your trip with add-ons like travel insurance and guided tours. Once payment is confirmed, you'll receive a booking confirmation via email.",
      viewText: false,
    },
    {
      question: "Do I need a visa for my destination?",
      answer: `LoremBuilt a system enabling companies to update website content (e.g., services, reviews) in real-time.
      Features include user authentication, content editing, and review approvals.
      Tools Used: FastAPI (Python), MongoDB, Svelte, JWT tokens.
    `,
      viewText: false,
    },
    {
      question: "Can I book flights for multiple destinations in one trip?",
      answer: `Built a system enabling companies to update website content (e.g., services, reviews) in real-time.
      Features include user authentication, content editing, and review approvals.
      Tools Used: FastAPI (Python), MongoDB, Svelte, JWT tokens.
      `,
      viewText: false,
    },
    {
      question: "How do I check baggage policies for different airlines?",
      answer: `Built a system enabling companies to update website content (e.g., services, reviews) in real-time.
      Features include user authentication, content editing, and review approvals.
      Tools Used: FastAPI (Python), MongoDB, Svelte, JWT tokens.
      "`,
      viewText: false,
    },
    {
      question: "What payment methods do you accept?",
      answer: `Built a system enabling companies to update website content (e.g., services, reviews) in real-time.
      Features include user authentication, content editing, and review approvals.
      Tools Used: FastAPI (Python), MongoDB, Svelte, JWT tokens.
      `,
      viewText: false,
    },
  ]);
</script>

<section class="mx-auto px-6 py-20 text-center">
  <!-- Header -->
  <h2 class="text-4xl font-semibold mb-3">
    <div class="mb-5">Wondering About❓</div>
    <div>Something?💡</div>
  </h2>
  <p class="text-gray-500 max-w-2xl mx-auto mb-12 text-2xl">
    From bookings to cancellations, find clear answers to all your
    travel-related concerns.
  </p>

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
