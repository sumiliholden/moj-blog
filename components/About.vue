<template>
  <div class="about">
    <h1>about component</h1>
    <button @click="backToHomeHandler()">Back to home component</button>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    backToHomeHandler() {
      const element = document.querySelector(".home");
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>
<style scoped>
.about {
  min-height: 100vh;
  background: red;
}
</style>
