<template>
  <article class="card">
    <nuxt-link
      :to="{ name: 'blog-slug'}"
      class="wrapper"
    >
      <h1 class="card_title">記事１</h1>
      <p class="card_text">記事の内容。ああああああああああああああああああ</p>
      <p class="card_date">2018/8/2</p>
    </nuxt-link>
  </article>
</template>

<style scoped>
.card {
  width: 300px;
  height: 200px;
  box-shadow: 1px 2px 3px 1px rgba(0, 0, 0, 0.2);
  border: 0.5px solid rgb(57, 72, 85);
  padding: 10px 20px;
  margin: 10px 10px;
}
.wrapper {
  text-decoration: none;
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
