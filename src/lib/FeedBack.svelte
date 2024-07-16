<script>
    // Mock data for feedbacks
    let feedbacks = [
      {
        name: 'Selphine Albert',
        exam: 'SBI PO 2023',
        feedback: 'Scoreclever saved my Current Affairs preparation time by 300%. Thanks team for making such a wonderful app.',
        rating: 5,
        image: 'src/assets/FeedBack Profile Pic/pic1.jpg'
      },
      {
        name: 'Shubam Yadav',
        exam: 'IBPS PO 2023',
        feedback: 'Scoreclever saved my Current Affairs preparation time by 300%. Thanks team for making such a wonderful app.',
        rating: 5,
        image: 'src/assets/FeedBack Profile Pic/pic1.jpg'
      },
      {
        name: 'Riyas Khan',
        exam: 'RBI Asst 2023',
        feedback: 'Scoreclever saved my Current Affairs preparation time by 300%. Thanks team for making such a wonderful app.',
        rating: 5,
        image: 'src/assets/FeedBack Profile Pic/pic4.JPG'
      },
      {
        name: 'Neha Dubey',
        exam: 'IBPS PO 2023',
        feedback: 'Scoreclever saved my Current Affairs preparation time by 300%. Thanks team for making such a wonderful app.',
        rating: 5,
        image: 'src/assets/FeedBack Profile Pic/pic3.jpg'
      }
    ];
  </script>
  
  <div class="p-4">
    <h2 class="text-xl font-bold mb-2">What aspirants say?</h2>
    <p class="text-green-500 mb-4">4.5 stars out of 1.5k ratings</p>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
      {#each feedbacks as feedback}
        <div class="bg-green-100 shadow-md rounded-lg p-6 text-center">
          <img src={feedback.image} alt={feedback.name} class="w-24 h-24 rounded-full mx-auto mb-4">
          <div class="flex justify-center mb-2">
            {#each Array(feedback.rating) as _}
              <svg class="w-6 h-6 text-green-500" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 .288l2.833 8.718h9.167l-7.417 5.385 2.833 8.718-7.416-5.384-7.417 5.384 2.833-8.718-7.417-5.385h9.167z"/>
              </svg>
            {/each}
          </div>
          <p class="font-bold">{feedback.name}</p>
          <p class="text-gray-500 mb-2">{feedback.exam}</p>
          <p class="text-gray-700">{feedback.feedback}</p>
        </div>
      {/each}
    </div>
  </div>
  