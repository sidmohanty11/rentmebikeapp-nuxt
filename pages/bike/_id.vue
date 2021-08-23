<template>
  <div class="container">
    <describe-id :bike="bike" />
    <customer-reviews />
  </div>
</template>

<script>
export default {
  computed: {
    bike() {
      return this.$store.getters.getBikeById(this.$route.params.id);
    }
  }
};
</script>
