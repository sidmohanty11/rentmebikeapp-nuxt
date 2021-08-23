<template>
  <div v-if="bike" class="container">
    <img
      height="400px"
      :src="require(`@/assets/img/${bike.image || 'b1.jpg'}`)"
      alt=""
    />
    <div class="container-para">
      <h1>{{ bike.title }}</h1>
      <p>
        {{ bike.snippet }}
      </p>
      <p>
        {{ bike.description }}
      </p>
      <p class="price-tag">Price - Rs. {{ bike.price }}/day</p>
      <a-button ghost> Rent me this! </a-button>
    </div>
  </div>
  <div v-else class="pagenotfound">Page Not Found</div>
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

<style scoped>
.container {
  margin: 20px 50px;
  display: flex;
  color: whitesmoke;
  justify-content: space-evenly;
  height: calc(100vh - 7em);
}
.container-para {
  width: 500px;
}

.container-para h1 {
  color: crimson;
}

.price-tag {
  color: aqua;
}

.pagenotfound {
  color: aqua;
}
</style>