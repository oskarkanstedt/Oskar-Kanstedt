<template>
  <nuxt-link :to="to" class="link"><slot /></nuxt-link>
</template>

<script>
export default {
  props: {
    to: String,
  },
}
</script>

<style scoped>
.link {
  color: green;
}
</style>
