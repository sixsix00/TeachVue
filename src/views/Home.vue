<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <LeftRightJumping />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import LeftRightJumping from "@/components/LeftRightJumping.vue";
export default {
  name: "Home",
  components: {
    HelloWorld,
    LeftRightJumping,
  },
};
</script>
