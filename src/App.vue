<template>
  <div class="h-screen flex flex-col">
    <header class="mt-10 w-full flex justify-center">
      <button
        @click.prevent="selected = 'COMPLETED'"
        class="px-2 py-1 mx-2 bg-transparent border rounded border-green-500 uppercase"
        :class="
          selected === 'COMPLETED'
            ? 'bg-green-500 text-white'
            : 'text-green-500'
        "
      >
        Completed
      </button>
      <button
        @click.prevent="selected = 'START'"
        class="px-2 py-1 mx-2 bg-transparent border rounded border-green-500 uppercase"
        :class="
          selected === 'START' ? 'bg-green-500 text-white' : 'text-green-500'
        "
      >
        START
      </button>
    </header>
    <main class="flex-grow flex justify-center items-center">
      <CardCompleted v-show="selected === 'COMPLETED'" />
      <CardStart v-show="selected === 'START'" />
    </main>
  </div>
</template>

<script>
import CardCompleted from "@/components/CardCompleted";
import CardStart from "@/components/CardStart";
export default {
  name: "App",
  components: { CardCompleted, CardStart },
  data() {
    return {
      selected: "START"
    };
  }
};
</script>

<style lang="postcss">
@tailwind base;

@tailwind components;

@tailwind utilities;
</style>
