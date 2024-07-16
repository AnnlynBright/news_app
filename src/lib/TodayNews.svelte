<script>
  import NewsCard from './NewsCard.svelte';

  const newsList = [
    {
      image: 'src/assets/Article/article-1.jpg', 
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    },
    {
      image: 'src/assets/Article/article-1.jpg',
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    },
    {
      image: 'src/assets/Article/article-1.jpg',
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    },
    {
      image: 'src/assets/Article/article-1.jpg',
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    },
    {
      image: 'src/assets/Article/article-1.jpg',
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    },
    {
      image: 'src/assets/Article/article-1.jpg',
      title: "UK election: What's happened and what comes next?",
      description: "Sir Keir Starmer’s Labour have won a big victory here's a guide to understanding what it all means.",
      readTime: '2 min',
      category: 'Politics'
    }
  ];
</script>

<main class="p-8 bg-gray-100">
  <h1 class="text-3xl font-bold mb-4 text-left">Top current affairs today</h1>
  <div class="grid gap-4 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-6">
      {#each newsList as news}
      <NewsCard image={news.image} title={news.title} description={news.description} readTime={news.readTime} category={news.category} />
      {/each}
  </div>
  <div class="flex justify-end mt-8">
      <button class="bg-green-600 text-white py-2 px-4 rounded-md hover:bg-green-700">Learn today's</button>
  </div>
</main>

<style>
  .overflow-x-auto {
      display: flex;
      flex-wrap: nowrap;
      overflow-x: auto;
      padding: 16px;
  }
</style>
