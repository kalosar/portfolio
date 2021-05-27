<template>
  <div class="flex flex-col bg-gray-900 bg-opacity-90 rounded-lg shadow">
    <div
      class="
        flex
        justify-between
        bg-gray-900
        rounded-t-lg
        px-2
        py-1
        text-gray-400 text-sm
        shadow
      "
    >
      <div class="flex items-center space-x-1.5 text-gray-700 fill-current">
        <icon-circle class="h-3 transition hover:text-red-500" />
        <icon-circle class="h-3 transition hover:text-yellow-500" />
        <icon-circle class="h-3 transition hover:text-green-500" />
      </div>
      <div class="select-none font-bold">Portfolio</div>
      <div />
    </div>

    <div class="flex flex-col flex-grow overflow-auto p-2 font-mono">
      <div v-for="item in history" :key="item" class="whitespace-pre-line">
        {{ item }}
      </div>
      <div>
        <span>kalosar@macbook></span>
        <span>{{ userInput }}</span>
        <span class="animate-ping font-bold">_</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ConsoleWindow',
  data() {
    return {
      history: [],
      prefix: 'kalosar@macbook> ',
      userInput: '',
      commands: {
        help:
          'Commands\n' +
          '--------\n' +
          '[help] ------- Print list of commands\n' +
          '[info] ------- Print info about me\n' +
          '[skills] ----- List skills\n' +
          '[experience] - List experience\n',
      },
    }
  },
  mounted() {
    this.history.push(this.commands.help)
  },
}
</script>

<style scoped></style>
