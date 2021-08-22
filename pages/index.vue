<template>
  <div>
    <carousel />
    <large-cards-holder
      v-for="cardInfo in info"
      :key="cardInfo.id"
      :info="cardInfo"
    />
    <small-cards-holder
      v-for="cardInfo in smallCardInfo"
      :key="cardInfo.id"
      :info="cardInfo"
    />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '~/assets/data';

export default {
  data() {
    return {
      info: largeCardSections,
      smallCardInfo: smallCardSections
    };
  }
};
</script>
