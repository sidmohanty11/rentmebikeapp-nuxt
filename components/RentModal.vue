<template>
  <div>
    <a-button ghost @click="showModal"> Rent Me this! </a-button>
    <a-modal v-model="visible" title="Choose Dates" @ok="handleOk">
      <div class="calendar-container">
        <div class="text-container">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus,
            illum.
          </p>
        </div>
      </div>
    </a-modal>
  </div>
</template>
<script>
export default {
  data() {
    return {
      visible: false
    };
  },
  methods: {
    showModal() {
      this.visible = true;
    },
    handleOk(e) {
      this.visible = false;
    }
  }
};
</script>
