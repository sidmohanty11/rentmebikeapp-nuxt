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
<script>
export default {};
</script>
<style scoped>
.ant-carousel >>> .slick-slide {
  text-align: center;
  height: calc(100vh - 20em);
  line-height: 160px;
  overflow: hidden;
}

.carousel-img-1 {
  height: calc(100vh - 20em);
  background-image: url('https://images.hdqwalls.com/wallpapers/electric-bike-4k-b9.jpg');
  background-size: cover;
}

.carousel-img-2 {
  height: calc(100vh - 20em);
  background-image: url('https://wallpaperaccess.com/full/3460572.jpg');
  background-size: cover;
}

.carousel-img-3 {
  height: calc(100vh - 20em);
  background-image: url('https://images.wallpaperscraft.com/image/bmw_k100_motorcycle_bike_123991_3840x2400.jpg');
  background-size: cover;
}

.carousel-img-4 {
  height: calc(100vh - 20em);
  background-image: url('https://www.wallpapersshare.com/img/big/black-yamaha-mt-07-bike-4k-photo.jpg');
  background-size: cover;
}

.ant-carousel >>> .slick-slide h3 {
  color: #fff;
  font-size: 30px;
}
</style>
