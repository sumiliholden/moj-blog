<template>
  <div>
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item href="#">Home</b-nav-item>
        <b-nav-item @click="aboutHandler()">About</b-nav-item>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data() {
    return {
      darwin: null,
    };
  },
  methods: {
    aboutHandler() {
      const element = document.querySelector(".about");
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>
