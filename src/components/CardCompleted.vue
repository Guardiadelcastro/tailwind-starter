<template>
  <div class="flex flex-col bg-white rounded overflow-hidden shadow-lg">
    <div>
      <img
        class="w-64 object-cover"
        src="https://images.unsplash.com/photo-1557330359-ffb0deed6163?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80"
        alt="crossfit img"
      />
    </div>
    <div class="px-3 py-2">
      <div class="flex justify-between">
        <h2 class="uppercase tracking-wider font-bold text-teal-500">
          100 Push-ups
        </h2>
        <p class="flex flex-col items-end">
          <span class="text-xs text-gray-700">Started on </span>
          <span class="text-indigo-500">May 16th</span>
        </p>
      </div>
      <div class="my-3 flex justify-between">
        <div class="text-sm text-gray-700">
          <p>Lowest</p>
          <p><span class="text-lg font-bold text-red-500">20</span> reps</p>
        </div>
        <div class="text-right text-sm text-gray-700">
          <p class="text-sm text-gray-700 ">Highest</p>
          <p><span class="text-lg font-bold text-teal-500">60</span> reps</p>
        </div>
      </div>
      <div class="border-t border-teal-200 text-center">
        <span class="text-2xl text-teal-400">+10</span
        ><span class="text-xl text-gray-700">Push ups</span
        ><span class="text-sm text-gray-500">/week</span>
      </div>
    </div>
    <div class="px-3 py-3 flex justify-end bg-gray-300">
      <button
        type="button"
        class="px-2 py-1 bg-teal-500 text-white rounded hover:bg-teal-400"
      >
        Continue challenge
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardCompleted"
};
</script>
