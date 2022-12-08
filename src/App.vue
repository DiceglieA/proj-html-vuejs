<template>
  <div>
    <HeaderComp />
    <MainComp />
    <FooterComp />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import MainComp from "./components/MainComp.vue"
import FooterComp from "./components/FooterComp.vue"

export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
    FooterComp
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

html {
  overflow-x: hidden;
}

ul {
  list-style-type: none;
}
a {
  text-decoration: none;
}
.violet {
    color: #4c4a9b;
}
</style>
