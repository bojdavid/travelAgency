<script lang="ts">
  const labelStyle: string = "text-[18px] text-gray-400";
</script>

<form class="w-[500px]">
  <div
    class="bg-white border border-gray-200 px-[50px] py-[10.5px] rounded-[16px] mb-8"
  >
    <div class="mb-5">
      <!-- Full Name -->
      <label for="full_name" class={labelStyle}>Full name</label>
      <input
        id="full_name"
        name="full_name"
        type="text"
        class="w-full border border-gray-300 px-4 py-2 rounded-[8px] focus:outline-none focus:ring-2 focus:ring-blue-400 bg-gray-100"
      />
    </div>
    <div class="mb-5">
      <!-- Email -->
      <label for="email" class={labelStyle}> Email</label>
      <input
        type="email"
        placeholder="Email"
        class="w-full border border-gray-300 px-4 py-2 rounded-[8px] focus:outline-none focus:ring-2 focus:ring-blue-400 bg-gray-100 h-[50px]"
      />
    </div>

    <!-- Phone + Subject -->
    <div class="flex gap-4 mb-5">
      <div>
        <label for="phoneNumber" class={labelStyle}>Phone Number</label>
        <!-- Country Code -->
        <div class="flex items-center border border-gray-300 rounded">
          <select
            class="bg-transparent px-2 outline-none text-3xl bg-gray-100 h-[50px] rounded-[8px]"
          >
            <option value="ng">🇳🇬</option>
          </select>
          <input
            type="tel"
            name="phoneNumber"
            id="phoneNumber"
            class="w-full px-2 py-2 outline-none text-sm bg-gray-100 h-[50px] rounded-[8px]"
          />
        </div>
      </div>

      <div>
        <!-- Subject -->
        <label for="subject" class={labelStyle}>Subject</label>
        <select
          class="w-full border border-gray-300 px-4 py-2 rounded-[8px] text-sm text-gray-400 focus:outline-none focus:ring-2 focus:ring-blue-400 bg-gray-100 h-[50px]"
          id="subject"
          name="subject"
        >
          <option>General inquiry</option>
          <option>Booking help</option>
          <option>Custom travel</option>
        </select>
      </div>
    </div>

    <div>
      <!-- Message -->
      <label for="message" class={labelStyle}>Message</label>
      <textarea
        name="message"
        id="message"
        class="w-full border border-gray-300 px-4 py-2 rounded-[8px] h-28 resize-none focus:outline-none focus:ring-2 focus:ring-blue-400 bg-gray-100 h-[120px]"
      ></textarea>
    </div>
  </div>

  <!-- Submit Button -->
  <div class="flex justify-center">
    <button
      class="bg-blue-600 text-white px-8 py-3 rounded-full hover:bg-blue-700 transition w-[300px] text-[24px]"
      >Submit</button
    >
  </div>
</form>
