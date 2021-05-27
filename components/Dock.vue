<template>
  <div
    class="
      flex
      items-center
      py-2
      px-6
      mb-2
      bg-gray-900 bg-opacity-90
      rounded-xl
      space-x-4
    "
  >
    <a href="https://github.com/kalosar" class="dock-button bg-black">
      <icon-github class="text-white fill-current" />
    </a>
    <a
      href="https://www.linkedin.com/in/marius-e-g-andresen/"
      class="dock-button bg-blue-500"
    >
      <icon-linkedin class="text-white fill-current" />
    </a>
  </div>
</template>

<script>
export default {
  name: 'Dock',
}
</script>

<style scoped>
.dock-button {
  @apply h-14 w-14 p-2 rounded-lg transform transition duration-500 hover:scale-110;
}
</style>
