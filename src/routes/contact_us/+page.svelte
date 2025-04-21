<script lang="ts">
  import Form from "$lib/components/contactUs/Form.svelte";
  import FAQ from "$lib/components/FAQ.svelte";

  interface Question {
    question: string;
    answer: string;
    viewText: boolean;
  }

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

<section class="bg-white text-gray-800 font-sans">
  <main class="w-[989.64px] mx-auto py-10 space-y-12">
    <!-- Top Contact Info Row -->
    <div class="flex justify-between text-[20px] items-center text-gray-700">
      <div class="flex justify-evenly gap-2">
        <span>📞 <strong>Call Us:</strong></span>
        <a href="tel:+2349038263356" class="text-blue-600">+234 903 826 3356</a>
      </div>
      <div class="flex items-center gap-2">
        <span>✉️ <strong>Email Us:</strong></span>
        <a href="mailto:SoarTravelagency@gmail.com" class="text-blue-600"
          >SoarTravelagency@gmail.com</a
        >
      </div>
      <div class="flex items-center gap-2">
        <span>🏷️ <strong>Our Socials:</strong></span>
        <div class="flex items-center gap-2 text-blue-600 text-lg">
          <a href="#">X</a>
          <a href="#">📷</a>
          <a href="#">▶️</a>
          <a href="#">📘</a>
        </div>
      </div>
    </div>

    <div class="w-[450px] mx-auto">
      <!-- Header Section -->
      <section class="text-center space-y-4 mb-5">
        <h1 class="text-[28px] font-semibold">Get in Touch</h1>
        <p class="text-gray-500 max-w-xl mx-auto text-[18px] leading-[27px]">
          Have questions, need assistance, or want to customize your travel
          experience? Please fill out this form and we'll get back to you as
          soon as possible.
        </p>
      </section>

      <!-- Contact Form -->
      <section class="flex justify-center mb-30">
        <Form />
      </section>
    </div>

    <!-- FAQ -->
    <section class="my-20">
      <!-- Header -->
      <h2 class="text-4xl font-semibold mb-3 text-center">
        <div class="mb-2">FAQs</div>
      </h2>
      <p
        class="text-gray-500 w-[343px] mx-auto mb-10 text-2xl text-center text-[18px]"
      >
        Find everything you need to know about bookings, travel policies and
        more
      </p>

      <FAQ {questions} />
    </section>
  </main>
</section>
