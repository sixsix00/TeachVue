<template>
  <div class="jumpBorder">
    <div :class="['leftDiv', { active: bbb }]">asdfasfss</div>
    <div :class="['rightDiv', { active: bbb }]">afdsasfsfsdafs</div>
  </div>
  <button @click="aaa">出現吧!</button>
</template>
<script>
import { ref } from "vue";
export default {
  name: "LeftRightJumping",
  props: {},
  setup() {
    const bbb = ref(false);
    const aaa = () => {
      bbb.value = bbb.value == false ? true : false;
      console.log(bbb.value);
    };

    return {
      aaa,
      bbb,
    };
  },
};
</script>
<style lang="scss">
@import "@/assets/scss/leftright.scss";
</style>