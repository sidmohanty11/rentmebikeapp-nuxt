<template>
  <div>
    <h1 class="heading-large-card-div">{{ info.title }}</h1>
    <h3>{{ info.snippet }}</h3>
    <div class="large-card-div">
      <card v-for="card in info.cards" :key="card.id" :card="card" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    info: {
      type: Object,
      required: true
    }
  }
};
</script>

<style scoped>
.heading-large-card-div {
  color: whitesmoke;
  font-size: 40px;
  text-align: center;
}

.large-card-div {
  margin: 40px;
  display: flex;
  justify-content: space-evenly;
}

h3 {
  color: whitesmoke;
  text-align: center;
}
</style>
