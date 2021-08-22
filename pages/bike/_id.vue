<template>
  <div class="container">
    <img height="400px" src="~/assets/img/b19.jpg" alt="" />
    <div class="container-para">
      <h1>Duke RC 200</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis ipsum
        voluptas nisi ab facere eum reiciendis, aspernatur quos, nobis explicabo
        officiis sed dolorum iste doloribus sapiente atque labore suscipit odit.
        Quo officia eos accusantium. Eius aspernatur corporis earum nulla
        voluptas quasi corrupti modi asperiores accusantium similique blanditiis
        officia, quaerat, optio delectus fuga neque minus eligendi laboriosam
        esse dolor enim facere! Esse, repellat accusamus. Mollitia, sapiente
        vero? Sed, in, ex sapiente consequatur et, pariatur excepturi provident
        aperiam inventore fugit adipisci numquam vel vero illum minus vitae
        magnam. Ad quae voluptates aspernatur? Modi quos ipsam veritatis velit
        cumque optio, quae beatae veniam doloremque nobis temporibus quod
        doloribus sunt, natus in accusantium.
      </p>
      <p class="price-tag">Price - Rs. 2000/day</p>
      <a-button ghost> Rent me this! </a-button>
    </div>
  </div>
</template>

<script>
export default {
  // computed: {
  //   bike() {
  //     return
  //   }
  // }
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
</style>