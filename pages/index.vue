<template>
  <section class="index">
    <card
      v-for="i in 5"
      :key="i"
    />
  </section>
</template>

<script>
import Card from '~/components/card.vue'

export default {
  components: {
    Card
  }
}
</script>

<style scoped>
.index {
  display: flex;
  flex-wrap: wrap;
}
</style>
