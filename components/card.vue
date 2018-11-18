<template>
  <nuxt-link
    :to="{ name: 'blog-slug', params: {
      sys: id
    }}"
    class="wrapper"
  >
    <article class="card">
      <h1 class="card_title">{{ title }}</h1>
      <p class="card_text">{{ id }}</p>
      <p class="card_date">{{ date }}</p>
    </article>
  </nuxt-link>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    id: {
      type: String,
      default: ''
    },
    date: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>
.card {
  width: 300px;
  height: 200px;
  box-shadow: 1px 2px 3px 1px rgba(0, 0, 0, 0.2);
  border: 0.5px solid rgb(57, 72, 85);
  padding: 10px 20px;
  margin: 10px 10px;
}
.card_title {
  font-size: 1.2rem;
}
.card_text {
  color: rgb(57, 72, 85);
  margin: 10px 0;
}
.card_date {
  font-size: 0.7rem;
  color: rgb(57, 72, 85);
  text-align: right;
}
</style>
