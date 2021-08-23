<template>
  <div class="container">
    <h3>Customer Reviews</h3>
    <div v-if="reviews.results">
      <review-card
        v-for="review in reviews.results"
        :key="review.login.uuid"
        :review="review"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      reviews: []
    };
  },
  async fetch() {
    this.reviews = await fetch(
      `https://randomuser.me/api/?results=${Math.floor(Math.random() * 10) + 5}`
    ).then((res) => res.json());
  }
};
</script>

<style scoped>
.container {
  text-align: center;
}
h3 {
  color: whitesmoke;
}
</style>