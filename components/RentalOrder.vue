<template>
  <div class="my-orders-cards">
    <a-card :title="rental.title">
      <a slot="extra" href="#">View Details</a>
      <img
        width="200px"
        height="100px"
        :src="require(`~/assets/img/${rental.image}`)"
        alt=""
      />
      {{ rental.snippet }}
      <p>Rs. {{ rental.price }}/day</p>
    </a-card>
  </div>
</template>

<script>
export default {
  props: {
    rental: {
      type: Object,
      default: () => {}
    }
  }
};
</script>

<style scoped>
.my-orders-cards {
  margin: 50px;
}
</style>