<script>
  import logo from '../assets/scvr_logo_top_bar.png'; // Update with the correct path
  import profilePic from '../assets/image.png'; // Update with the correct path
</script>

<style>
  .toggle-button {
      position: relative;
      display: inline-block;
      width: 34px;
      height: 20px;
  }

  .toggle-button input {
      opacity: 0;
      width: 0;
      height: 0;
  }

  .toggle-bg {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: #ccc;
      border-radius: 34px;
  }

  .toggle-dot {
      position: absolute;
      bottom: 2px;
      left: 2px;
      width: 16px;
      height: 16px;
      background-color: white;
      border-radius: 50%;
      transition: transform 0.2s;
  }

  input:checked + .toggle-bg {
      background-color: #4caf50;
  }

  input:checked + .toggle-bg + .toggle-dot {
      transform: translateX(14px);
  }
</style>

<header class="fixed top-0 left-0 w-full flex justify-between items-center p-4 bg-white shadow-md z-50">
  <div class="flex items-center space-x-4">
      <img src={logo} alt="Logo" class="h-10">
      <nav class="flex space-x-8 ml-8">
          <a href="/learn" class="text-green-600 hover:text-green-800">Learn</a>
          <a href="/download" class="text-green-600 hover:text-green-800">Download</a>
          <a href="/memorize" class="text-green-600 hover:text-green-800">Memorize</a>
          <a href="/performance" class="text-green-600 hover:text-green-800">Performance</a>
      </nav>
  </div>
  <div class="flex items-center space-x-4">
      <label class="toggle-button">
          <input type="checkbox">
          <span class="toggle-bg"></span>
          <span class="toggle-dot"></span>
      </label>
      <img src="/path/to/world-icon.png" alt="World Icon" class="h-6"> <!-- Update with the correct path -->
      <img src={profilePic} alt="Profile" class="h-10 rounded-full">
  </div>
</header>
