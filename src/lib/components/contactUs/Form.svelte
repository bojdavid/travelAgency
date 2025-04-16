<script lang="ts">
</script>

<form
  class="w-[480px] bg-white border border-gray-200 p-6 rounded-lg space-y-4"
>
  <!-- Full Name -->
  <input
    type="text"
    placeholder="Full name"
    class="w-full border border-gray-300 px-4 py-2 rounded focus:outline-none focus:ring-2 focus:ring-blue-400"
  />

  <!-- Email -->
  <input
    type="email"
    placeholder="Email"
    class="w-full border border-gray-300 px-4 py-2 rounded focus:outline-none focus:ring-2 focus:ring-blue-400"
  />

  <!-- Phone + Subject -->
  <div class="flex gap-4">
    <!-- Country Code -->
    <div class="flex items-center border border-gray-300 rounded px-2">
      <select class="bg-transparent py-2 outline-none text-sm">
        <option value="ng">🇳🇬</option>
      </select>
      <input
        type="tel"
        placeholder="Phone number"
        class="w-full px-2 py-2 outline-none text-sm"
      />
    </div>

    <!-- Subject -->
    <select
      class="w-full border border-gray-300 px-4 py-2 rounded text-sm focus:outline-none focus:ring-2 focus:ring-blue-400"
    >
      <option>General inquiry</option>
      <option>Booking help</option>
      <option>Custom travel</option>
    </select>
  </div>

  <!-- Message -->
  <textarea
    placeholder="Message"
    class="w-full border border-gray-300 px-4 py-2 rounded h-28 resize-none focus:outline-none focus:ring-2 focus:ring-blue-400"
  ></textarea>
</form>
