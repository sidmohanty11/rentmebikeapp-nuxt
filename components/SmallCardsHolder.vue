<template>
  <div>
    <h1 class="heading-small-card-div">{{ info.title }}</h1>
    <div class="small-card-div">
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
.heading-small-card-div {
  color: whitesmoke;
  font-size: 40px;
  text-align: center;
}

.small-card-div {
  margin: 40px;
  display: grid;
  grid-template-columns: 300px 300px 300px;
  grid-template-rows: 300px 300px 300px;
  column-gap: 10px;
  row-gap: 15px;
  justify-content: space-evenly;
}

h3 {
  color: whitesmoke;
  text-align: center;
}
</style>
