<template>
  <div>
    <a-card style="width: 300px">
      <img
        slot="cover"
        alt="bikes"
        :src="require(`@/assets/img/${card.image || 'b1.jpg'}`)"
      />
      <a-card-meta :title="card.title">
        <template slot="description">{{ card.snippet || null }}</template>
      </a-card-meta>
      <p class="price-tag">{{ card.price || null }}</p>
      <nuxt-link :to="`/bike/${card.id}`">View More</nuxt-link>
    </a-card>
  </div>
</template>

<script>
export default {
  props: {
    card: {
      type: Object,
      default: () => {}
    }
  }
};
</script>

<style scoped>
.ant-card {
  background-color: #f2f2f2;
  padding: 10px;
  border-color: black;
}
.price-tag {
  color: red;
}
</style>