<template>
  <div>
    <a-button ghost @click="showModal"> Rent Me this! </a-button>
    <a-modal
      v-model="visible"
      title="Choose Dates"
      @ok="
        () => {
          addItem(id);
          visible = false;
        }
      "
    >
      <div class="calendar-container">
        <div class="text-container">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus,
            illum.
          </p>
        </div>
        <vc-calendar :value="null" color="indigo" is-dark is-range />
      </div>
    </a-modal>
  </div>
</template>
<script>
import { mapMutations } from 'vuex';
export default {
  props: {
    id: {
      type: Number,
      required: true
    }
  },
  data() {
    return {
      visible: false
    };
  },
  methods: {
    showModal() {
      this.visible = true;
    },
    ...mapMutations(['addItem'])
  }
};
</script>

<style scoped>
.calendar-container {
  display: flex;
  justify-content: center;
}
</style>