<template>
  <div>
    <!-- <TitleComp /> -->
    <WelcomeComp />
    <!-- <TitleComp /> -->
    <ClassesComp />
  </div>
</template>

<script>
import WelcomeComp from './WelcomeComp.vue';
import ClassesComp from './ClassesComp.vue';
// import TitleComp from ".components/TitleComp.vue";

export default {
name: 'MainComp',
components: {
    WelcomeComp,
    ClassesComp,
    //  TitleComp,
},
//  data() {
//      return {
//        arrTitle: [
//          {
//            title: 'Welcome to Fable',
//            subtitle: 'Fable daycare, preschool, and kindergarten',
//            image: '"../assets/img/images/header_divider.png"'
//          },
//          {
//            title: 'Our Classes',
//            subtitle: 'Our preschool program has four dedicated classes',
//            image: '"../assets/img/images/header_divider.png"'
//          },
//          {
//            title: 'Meet Our Staff',
//            subtitle: 'With education and experience in early childhood care',
//            image: '"../assets/img/images/header_divider.png"'
//          },
//          {
//            title: 'What s New',
//            subtitle: 'Keep up to date with the latest news',
//            image: '"../assets/img/images/header_divider.png"'
//          },
//          {
//            title: 'Contact Us',
//            subtitle: 'Our postal address and contact detail',
//            image: '"../assets/img/images/header_divider.png"'
//          },
//        ]
//      }
//    }
}
</script>

<style lang="scss" scoped>

</style>