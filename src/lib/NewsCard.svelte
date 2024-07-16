<script>
  export let image;
  export let title;
  export let description;
  export let readTime;
  export let category;
</script>

<div class="max-w-xs min-w-xs rounded overflow-hidden shadow-lg m-4">
  <!-- svelte-ignore a11y-img-redundant-alt -->
  <img class="w-full h-100" src={image} alt="News Image">
  <div class="px-4 py-2">
    <div class="font-bold text-xl mb-2">{title}</div>
    <p class="text-gray-700 text-base">{description}</p>
  </div>
  <div class="px-6 pt-4 pb-2">
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{readTime} read</span>
    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{category}</span>
  </div>
</div>

<style>
  .min-w-xs {
    min-width: 200px;
  }
</style>

<!-- Accessibility Note: Screen readers already announce <img> elements as an image. -->
