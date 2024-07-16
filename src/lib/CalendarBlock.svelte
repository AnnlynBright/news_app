<!-- <script>
    import QRcode from "../assets/qr-code 1.jpg";
  </script>
  
  <main>
    <section class=" flex  flex-col w-full p-2 bg-green-100 mt-16">
    <div >
      <h2 class="text-xl font-bold mb-4">Our expert team 🏅 has covered</h2>
      <ul class="space-y-2">
        <li class="flex items-center space-x-2">
          <span class="text-blue-600">🌍</span>
          <span>23 news today</span>
        </li>
        <li class="flex items-center space-x-2">
          <span class="text-blue-600">🌍</span>
          <span>142 news this week</span>
        </li>
        <li class="flex items-center space-x-2">
          <span class="text-blue-600">🌍</span>
          <span>4261 news this month</span>
        </li>
      </ul>
      <p class="mt-4 text-sm text-gray-600">Meticulously crafted from 4 newspapers - The Hindu, The New Indian Express, Business Standard, Mint, and the PIB</p>
      <div class="flex items-center mt-4 space-x-4">
        <img src="/images/logo/bst.jpg" alt="The Hindu" class="h-8">
        <img src="/images//logo/hindu.png" alt="The Indian Express" class="h-8">
        <img src="/images/business-standard-logo.png" alt="Business Standard" class="h-8">
        <img src="/images/mint-logo.png" alt="Mint" class="h-8">
        <img src="/images/pib-logo.png" alt="PIB" class="h-8">
      </div>
    </div>
    <div>
      <h2 class="text-xl font-bold mb-4">Pick a date to learn 🗓️</h2>
      <input type="text" id="calendar" class="border border-gray-300 rounded-md p-2 mb-4">
      <button id="learn-button" class="bg-green-600 text-white py-2 px-4 rounded-md hover:bg-green-700">Learn</button>
    </div>
  </section>
  </main> -->
<!-- 
  <script>
    import QRcode from "../assets/qr-code 1.jpg";
</script>

<main class="flex justify-center top-0 left-0 items-center flex-col w-full p-2 bg-green-10 mt-16">
  <div class="bg-white p-4 top-0 left-0 rounded-md max-w-7xl w-full flex justify-between items-center">
    <div class="flex-grow p-4 bg-green-100 rounded-md">
      <h1 class="text-2xl font-bold mb-4 text-black">Our expert team 🏅 has covered</h1>
      <ul class="space-y-2">
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">23 news today</span>
        </li>
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">142 news this week</span>
        </li>
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">4261 news this month</span>
        </li>
      </ul>
      <p class="mt-4 text-sm text-gray-600">Meticulously crafted from 4 newspapers - The Hindu, The New Indian Express, Business Standard, Mint, and the PIB</p>
      <div class="flex items-center mt-4 space-x-4">
        <img src="/images/logo/bst.jpg" alt="The Hindu" class="h-8">
        <img src="/images/logo/hindu.png" alt="The Indian Express" class="h-8">
        <img src="/images/business-standard-logo.png" alt="Business Standard" class="h-8">
        <img src="/images/mint-logo.png" alt="Mint" class="h-8">
        <img src="/images/pib-logo.png" alt="PIB" class="h-8">
      </div>
    </div>
    <div class="flex flex-col items-center p-4 ml-4 bg-green-100 rounded-md">
      <h1 class="text-2xl font-bold mb-4 text-black">Pick a date to learn 🗓️</h1>
      <input type="text" id="calendar" class="border border-gray-300 rounded-md p-2 mb-4">
      <button id="learn-button" class="bg-green-600 text-white py-2 px-4 rounded-md hover:bg-green-700">Learn</button>
    </div>
  </div>
</main> -->
<!-- 
<script>
  import QRcode from "../assets/qr-code 1.jpg";
  import flatpickr from "flatpickr";
  import "flatpickr/dist/flatpickr.css";
  import { onMount } from "svelte";

  let calendarDiv;

  onMount(() => {
    flatpickr(calendarDiv, {
      inline: true, // Display the calendar inline
      dateFormat: "Y-m-d",
    });
  });
</script>

<main class="flex justify-center top-0 left-0 items-center flex-col w-full p-2 bg-green-10 mt-16">
  <div class="bg-white p-4 top-0 left-0 rounded-md max-w-7xl w-full flex justify-between items-center">
    <div class="flex-grow p-4 bg-green-100 rounded-md">
      <h1 class="text-2xl font-bold mb-4 text-black">Our expert team 🏅 has covered</h1>
      <ul class="space-y-2">
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">23 news today</span>
        </li>
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">142 news this week</span>
        </li>
        <li class="flex items-start space-x-2">
          <span class="text-blue-600">🌍</span>
          <span class="text-black">4261 news this month</span>
        </li>
      </ul>
      <p class="mt-4 text-sm text-gray-600">Meticulously crafted from 4 newspapers - The Hindu, The New Indian Express, Business Standard, Mint, and the PIB</p>
      <div class="flex items-center mt-4 space-x-4">
        <img src="/images/logo/bst.jpg" alt="The Hindu" class="h-8">
        <img src="/images/logo/hindu.png" alt="The Indian Express" class="h-8">
        <img src="/images/business-standard-logo.png" alt="Business Standard" class="h-8">
        <img src="/images/mint-logo.png" alt="Mint" class="h-8">
        <img src="/images/pib-logo.png" alt="PIB" class="h-8">
      </div>
    </div>
    <div class="flex flex-col items-center p-4 ml-4 bg-green-100 rounded-md">
      <h1 class="text-2xl font-bold mb-4 text-black">Pick a date to learn 🗓️</h1>
      <div bind:this={calendarDiv} class="border border-gray-300 rounded-md p-2 mb-4"></div>
      <button id="learn-button" class="bg-green-600 text-white py-2 px-4 rounded-md hover:bg-green-700">Learn</button>
    </div>
  </div>
</main> -->

<script>
  import QRcode from "../assets/qr-code 1.jpg";
  import flatpickr from "flatpickr";
  import "flatpickr/dist/flatpickr.css";
  import { onMount } from "svelte";

  let calendarDiv;

  onMount(() => {
    flatpickr(calendarDiv, {
      inline: true, // Display the calendar inline
      dateFormat: "Y-m-d",
    });
  });
</script>

<main class="flex justify-center top-0 left-0 items-center flex-col w-full p-2 bg-green-10 mt-16">
  <div class="bg-white p-4 top-0 left-0 rounded-md max-w-7xl w-full flex justify-between items-stretch">
    <div class="flex-grow p-10 bg-green-100 rounded-md flex flex-col justify-between">
      <div>
        <h1 class="text-2xl font-bold mb-4 text-black">Our expert team 🏅 has covered</h1>
        <ul class="space-y-2">
          <li class="flex items-start space-x-2">
            <span class="text-blue-600">🌍</span>
            <span class="text-black font-bold">23 news today</span>
          </li>
          <li class="flex items-start space-x-2">
            <span class="text-blue-600">🌍</span>
            <span class="text-black font-bold">142 news this week</span>
          </li>
          <li class="flex items-start space-x-2">
            <span class="text-blue-600">🌍</span>
            <span class="text-black font-bold">4261 news this month</span>
          </li>
        </ul>
        <p class="mt-4 text-sm text-black font-bold">Meticulously crafted from 4 newspapers - The Hindu, The New <br> Indian Express, Business Standard, Mint, and the PIB</p>
      </div>
      <div class="flex items-center mt-4 space-x-4">
        <img src="src/assets/news_logo/the hindu 1.png" alt="The Hindu" class="h-8">
        <img src="src/assets/news_logo/tiex 1.png"alt="The Indian Express" class="h-8">
        <img src="src/assets/news_logo/bstd 1.jpg" alt="Business Standard" class="h-8">
        <img src="src/assets/news_logo/mint 1.png" alt="Mint" class="h-8">
        <img src="src/assets/news_logo/pib 1.png" alt="PIB" class="h-8">
      </div>
    </div>
    <div class="flex flex-col items-center p-4 ml-4 bg-green-100 rounded-md flex-grow">
      <h1 class="text-2xl font-bold mb-4 text-black">Pick a date to learn 🗓️</h1>
      <div bind:this={calendarDiv} class="border border-gray-300 rounded-md p-2 mb-4"></div>
      <button id="learn-button" class="bg-green-600 text-white p-2 py-2 px-4 rounded-md hover:bg-green-700 ">Learn</button>
    </div>
  </div>
</main>


