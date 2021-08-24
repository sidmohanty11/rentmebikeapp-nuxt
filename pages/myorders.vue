<template>
  <div class="container">
    <rental-order
      v-for="myRental in myRentals"
      :key="myRental.id"
      :rental="myRental"
    />
  </div>
</template>

<script>
export default {
  computed: {
    myRentals() {
      return this.$store.getters.getMyRentals;
    }
  }
};
</script>

<style scoped>
.container {
  min-height: calc(100vh - 4em);
}
</style>