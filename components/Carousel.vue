<template>
  <a-carousel autoplay>
    <div class="carousel-img-1">
      <h3>“My prince charming doesn’t ride a horse…he rides wheelies.”</h3>
    </div>
    <div class="carousel-img-2">
      <h3>“Four wheels move the body, Two wheels move the soul.”</h3>
    </div>
    <div class="carousel-img-3">
      <h3>
        “Faster, faster, faster, until the thrill of speed overcomes the fear of
        death.”
      </h3>
    </div>
    <div class="carousel-img-4">
      <h3>“I don’t need a therapy, I just need to ride my bike.”</h3>
    </div>
  </a-carousel>
</template>

<style scoped>
.ant-carousel >>> .slick-slide {
  text-align: center;
  height: calc(100vh - 20em);
  line-height: 160px;
  overflow: hidden;
}

.carousel-img-1 {
  height: calc(100vh - 20em);
  background-image: url('~assets/img/3.jpg');
  background-size: cover;
}

.carousel-img-2 {
  height: calc(100vh - 20em);
  background-image: url('~assets/img/2.jpg');
  background-size: cover;
}

.carousel-img-3 {
  height: calc(100vh - 20em);
  background-image: url('~assets/img/4.jpg');
  background-size: cover;
}

.carousel-img-4 {
  height: calc(100vh - 20em);
  background-image: url('~assets/img/1.jpg');
  background-size: cover;
}

.ant-carousel >>> .slick-slide h3 {
  color: #fff;
  font-size: 30px;
}
</style>
