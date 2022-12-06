<template>
  <div>
    <HeaderComp />
    <MainComp />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import MainComp from "./components/MainComp.vue"
export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
  },
};
</script>

<style lang="scss">

@import "~bootstrap/scss/bootstrap";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

ul {
  list-style-type: none;
}
a {
  text-decoration: none;
}
</style>
