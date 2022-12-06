<template>
  <div>
    <HeaderComp />
    
    <MainComp />
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
// import TitleComp from ".components/TitleComp.vue";
import MainComp from "./components/MainComp.vue"
export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
    // TitleComp,
  },
  // data() {
  //   return {
  //     arrTitle: [
  //       {
  //         title: 'Welcome to Fable',
  //         subtitle: 'Fable daycare, preschool, and kindergarten',
  //         image: '"../assets/img/images/header_divider.png"'
  //       },
  //       {
  //         title: 'Our Classes',
  //         subtitle: 'Our preschool program has four dedicated classes',
  //         image: '"../assets/img/images/header_divider.png"'
  //       },
  //       {
  //         title: 'Meet Our Staff',
  //         subtitle: 'With education and experience in early childhood care',
  //         image: '"../assets/img/images/header_divider.png"'
  //       },
  //       {
  //         title: 'What s New',
  //         subtitle: 'Keep up to date with the latest news',
  //         image: '"../assets/img/images/header_divider.png"'
  //       },
  //       {
  //         title: 'Contact Us',
  //         subtitle: 'Our postal address and contact detail',
  //         image: '"../assets/img/images/header_divider.png"'
  //       },
  //     ]
  //   }
  // }
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
