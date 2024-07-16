<script>
  import QRcode from "../assets/qr-code 1.jpg";
</script>

<main class="flex justify-center top-0 left-0 items-center flex-col w-full p-2 bg-green-10 mt-16">
  <div class="bg-white p-4 top-0 left-0 rounded-md max-w-7xl w-full flex justify-between items-center">
      <div class="flex-grow p-4 bg-green-100 rounded-md">
          <h1 class="text-2xl font-bold mb-4 text-black">Welcome to Scoreclever 🕰 Current Affairs 🌍</h1>
          <ul class="space-y-2">
              <li class="flex items-start space-x-2">
                  <span class="text-gray-500">👉</span>
                  <span class="text-black">Detailed daily current affairs on website</span>
              </li>
              <li class="flex items-start space-x-2">
                  <span class="text-gray-500">👉</span>
                  <span class="text-black">Crisp current affairs on daily PDFs</span>
              </li>
              <li class="flex items-start space-x-2">
                  <span class="text-gray-500">👉</span>
                  <span class="text-black">Easy memorization and revision with app</span>
              </li>
          </ul>
          <div class="mt-4 justify-center ">
              <button class="bg-green-600  text-white py-2 px-4 rounded-md hover:bg-green-700">Download PDFs</button>
          </div>
      </div>
      <div class="flex flex-col items-center p-4 ml-4 bg-green-100 rounded-md">
          <img src={QRcode} alt="QR Code to download app" class="h-40 mb-4">
          <button class="bg-green-600 text-white py-2 px-4 rounded-md hover:bg-green-700">Download App</button>
      </div>
  </div>
</main>
