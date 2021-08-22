<template>
  <div>
    <h1 class="heading-large-card-div">{{ title }}</h1>
    <div class="large-card-div">
      <card />
      <card />
      <card />
      <card />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
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
</style>
