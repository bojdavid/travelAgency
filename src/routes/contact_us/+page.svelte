<script lang="ts">
  import Form from "$lib/components/contactUs/Form.svelte";
</script>

<section class="bg-white text-gray-800 font-sans">
  <main class="w-[989.64px] mx-auto px-6 py-10 space-y-12">
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

    <div class="w-[500px] mx-auto">
      <!-- Header Section -->
      <section class="text-center space-y-4">
        <h1 class="text-2xl font-semibold">Get in Touch</h1>
        <p class="text-gray-500 max-w-xl mx-auto text-sm">
          Have questions, need assistance, or want to customize your travel
          experience? Please fill out this form and we’ll get back to you as
          soon as possible.
        </p>
      </section>

      <!-- Contact Form -->
      <section class="flex justify-center">
        <Form />
      </section>

      <!-- Submit Button -->
      <div class="flex justify-center">
        <button
          class="bg-blue-600 text-white px-8 py-3 rounded-full hover:bg-blue-700 transition"
          >Submit</button
        >
      </div>
    </div>
  </main>
</section>
