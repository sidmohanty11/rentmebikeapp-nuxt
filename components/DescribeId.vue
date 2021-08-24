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
      <rent-modal :id="bike.id" />
    </div>
  </div>
</template>

<script>
import RentModal from './RentModal.vue';
export default {
  components: { RentModal },
  props: {
    bike: {
      type: Object,
      required: true
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