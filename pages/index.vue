<template>
  <div
    class="flex flex-col h-screen w-screen bg-cover"
    style="background-image: url(/bg-work-harder.jpg)"
  >
    <!-- Top Bar -->
    <header
      class="
        h-8
        flex
        items-center
        justify-between
        py-2
        px-4
        bg-gray-900 bg-opacity-90
        text-gray-400 text-sm
        shadow-lg
      "
    >
      <span>Marius Andresen</span>
      <date-time locale="en-GB" date="full" time="short" />
    </header>

    <!-- Main Content -->
    <main class="flex flex-grow items-center justify-center relative">
      <console-window />
    </main>

    <!-- Action Bar -->
    <footer class="flex justify-center">
      <dock />
    </footer>
  </div>
</template>

<script>
export default {}
</script>

<style scoped></style>
