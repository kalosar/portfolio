<template>
  <div
    class="
      flex flex-col
      h-screen
      w-screen
      bg-cover bg-gradient-to-br
      text-gray-400
      from-green-600
      to-blue-600
    "
  >
    <header
      class="
        h-8
        flex
        items-center
        justify-between
        py-2
        px-4
        bg-gray-900 bg-opacity-90
        text-sm
        shadow-lg
      "
    >
      <span>Marius Andresen</span>
      <date-time locale="en-GB" date="full" time="short" />
    </header>

    <main class="flex flex-grow items-center justify-center relative">
      <console-window class="h-5/6 w-1/2 absolute" />
    </main>

    <footer class="flex items-center justify-center mb-2">
      <dock />
    </footer>
  </div>
</template>

<script>
export default {}
</script>

<style scoped></style>
