<script>
    // Mock data for the leaderboard
    let leaderboard = [
      { id: 1, username: 'nv456789', score: 124 },
      { id: 2, username: 'logesh', score: 123.5 },
      { id: 3, username: 'yuvabala', score: 123.5 },
      // Add more users as needed
    ];
  
    let otherParticipants = [
      { id: 4, username: '@nithyasree1532001' },
      { id: 5, username: 'i' },
      { id: 6, username: '@padhu_99' },
      { id: 7, username: 'lalitha' },
      { id: 8, username: '@mrpk1708' },
      { id: 9, username: '@nithyasree1532001' },
      { id: 10, username: 'i' },
      { id: 11, username: '@padhu_99' },
      { id: 12, username: 'lalitha' },
      { id: 13, username: '@mrpk1708' },
      // Add more participants as needed
    ];
  </script>
  
  <style>
    /* Custom styles for the podium */
    .podium {
      display: flex;
      justify-content: center;
      align-items: flex-end;
      margin-bottom: 1rem;
    }
    .podium-step {
      background-color: #34D399;
      color: white;
      text-align: center;
      font-weight: bold;
      padding: 1rem;
      border-radius: 0.5rem 0.5rem 0 0;
    }
    .podium-step:nth-child(1) {
      height: 6rem;
      width: 6rem;
      margin: 0 1rem;
    }
    .podium-step:nth-child(2) {
      height: 8rem;
      width: 6rem;
      margin: 0 1rem;
    }
    .podium-step:nth-child(3) {
      height: 5rem;
      width: 6rem;
      margin: 0 1rem;
    }
  </style>
  
  <div class="p-4 bg-white shadow-md rounded-lg">
    <h2 class="text-lg font-bold mb-4">CA League Leaderboard</h2>
    <div class="flex">
      <div class="w-1/2">
        <div class="podium">
          <div class="podium-step">
            <img src="/path/to/image.png" alt="1st place" class="rounded-full w-16 h-16 mx-auto mb-2">
            {leaderboard[1].username}
            <div class="mt-1">{leaderboard[1].score}</div>
            <div class="mt-1">2</div>
          </div>
          <div class="podium-step">
            <img src="/path/to/image.png" alt="1st place" class="rounded-full w-16 h-16 mx-auto mb-2">
            {leaderboard[0].username}
            <div class="mt-1">{leaderboard[0].score}</div>
            <div class="mt-1">1</div>
          </div>
          <div class="podium-step">
            <img src="/path/to/image.png" alt="1st place" class="rounded-full w-16 h-16 mx-auto mb-2">
            {leaderboard[2].username}
            <div class="mt-1">{leaderboard[2].score}</div>
            <div class="mt-1">3</div>
          </div>
        </div>
      </div>
      <div class="w-1/2 grid grid-cols-3 gap-4">
        {#each otherParticipants as participant}
          <div class="flex items-center space-x-4">
            <div class="bg-gray-300 h-10 w-10 flex items-center justify-center rounded-full text-purple-700 font-bold">
              {participant.username[0]}
            </div>
            <div>
              <p class="font-semibold">{participant.username}</p>
            </div>
          </div>
        {/each}
      </div>
    </div>
  
    <div class="mt-6 bg-green-100 p-4 rounded-lg">
      <p>Current Affairs quizzes are conducted on our telegram channel at 8 PM everyday as a league. New League will start every month. Marks obtained by the participants are added from day 1 until the end of the month and top 3 winners will receive exciting rewards.</p>
      <button class="mt-4 justify-end bg-green-500  text-white px-4 py-2 rounded-lg">Join CA league</button>
    </div>
  </div>
  