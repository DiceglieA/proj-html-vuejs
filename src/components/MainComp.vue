<template>
  <div>
    <EnrollBar :datibars="purplebars[0]" />
    <TitleComp :datititle="arrtitle[0]" />
    <WelcomeComp />
    <TitleComp :datititle="arrtitle[1]" />
    <ClassesComp />
    <EnrollBar :datibars="purplebars[1]" />
    <TitleComp :datititle="arrtitle[2]" />
    <StaffComp />
  </div>
</template>

<script>
import EnrollBar from './EnrollBar.vue';
import WelcomeComp from './WelcomeComp.vue';
import ClassesComp from './ClassesComp.vue';
import StaffComp from './StaffComp.vue';
import TitleComp from "./TitleComp.vue";

export default {
name: 'MainComp',
components: {
    EnrollBar,
    WelcomeComp,
    ClassesComp,
    StaffComp,
    TitleComp,
},
data() {
  return {
  purplebars: [
      {
        title: 'How to Enroll Your Child to a class?',
        button: 'LEARN MORE'
      },
      {
        title: ' See Our Kindergarten Photo Gallery!',
        button: 'VIEW GALLERY'
      }
    ],
  arrtitle: [
      {
        title: 'Welcome to Fable',
        subtitle: 'Fable daycare, preschool, and kindergarten',
        image: 'header_divider.png'
      },
      {
        title: 'Our Classes',
        subtitle: 'Our preschool program has four dedicated classes',
        image: 'header_divider.png'
      },
      {
        title: 'Meet Our Staff',
        subtitle: 'With education and experience in early childhood care',
        image: 'header_divider.png'
      },
      {
        title: 'What s New',
        subtitle: 'Keep up to date with the latest news',
        image: 'header_divider.png'
      },
      {
        title: 'Contact Us',
        subtitle: 'Our postal address and contact detail',
        image: 'header_divider.png'
      },
    ]
  }
}
}
</script>

<style lang="scss" scoped>

</style>