<template>
  <div class="flex items-center space-x-1 select-none">
    <time>{{ localizedDate }}</time>
    <icon-calendar type="solid" class="h-5 w-5" />
    <div />
    <time>{{ localizedTime }}</time>
    <icon-clock type="solid" class="h-5 w-5" />
  </div>
</template>

<script>
export default {
  name: 'DateTime',
  props: {
    locale: {
      required: false,
      type: String,
      default: 'en-GB',
    },
    date: {
      required: false,
      type: String,
      default: 'short',
      validator(value) {
        return (
          value === 'short' ||
          value === 'medium' ||
          value === 'long' ||
          value === 'full'
        )
      },
    },
    time: {
      required: false,
      type: String,
      default: 'short',
      validator(value) {
        return (
          value === 'short' ||
          value === 'medium' ||
          value === 'long' ||
          value === 'full'
        )
      },
    },
  },
  data() {
    return {
      now: Date.now(),
    }
  },
  computed: {
    localizedDate() {
      const options = { dateStyle: this.date }
      return new Intl.DateTimeFormat(this.locale, options).format(this.now)
    },
    localizedTime() {
      const options = { timeStyle: this.time }
      return new Intl.DateTimeFormat(this.locale, options).format(this.now)
    },
  },
  created() {
    setInterval(() => (this.now = Date.now()), 1000)
  },
  destroyed() {
    clearInterval()
  },
}
</script>

<style scoped></style>
