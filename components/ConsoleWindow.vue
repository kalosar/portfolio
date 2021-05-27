<template>
  <div
    class="
      z-10
      h-5/6
      w-1/2
      absolute
      flex flex-col
      bg-gray-900 bg-opacity-90
      rounded-lg
      shadow-lg
    "
  >
    <div
      class="
        z-20
        flex
        justify-between
        bg-gray-900
        rounded-t-lg
        px-2
        py-1
        text-gray-400 text-sm
      "
    >
      <div class="flex items-center space-x-1.5 text-gray-700 fill-current">
        <icon-circle class="h-3 transition hover:text-red-500" />
        <icon-circle class="h-3 transition hover:text-yellow-500" />
        <icon-circle class="h-3 transition hover:text-green-500" />
      </div>
      <div class="select-none">Portfolio</div>
      <div class="select-none"></div>
    </div>
    <div
      class="flex flex-col flex-grow overflow-auto p-2 text-gray-400 font-mono"
    >
      <div>
        <ul>
          <li v-html="commands.help" />
        </ul>
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
      userInput: '',
      commands: {
        help:
          '<p>Commands</p>\n' +
          '<p>--------</p>\n' +
          '<p>[h]|[help] ------- Print list of commands</p>\n' +
          '<p>[i]|[info] ------- Print info about me</p>\n' +
          '<p>[s]|[skills] ----- List skills</p>\n' +
          '<p>[e]|[experience] - List experience</p>\n' +
          '<br />\n' +
          '</div>',
      },
    }
  },
}
</script>

<style scoped></style>
