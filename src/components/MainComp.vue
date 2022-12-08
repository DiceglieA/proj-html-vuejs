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
    <TitleComp :datititle="arrtitle[3]" />
    <div class="row container-80">
      <NewsComp v-for="(elem, index) in postcards" :key="index" :post="postcards[index]" class="col-4"/>
    </div>
    <a href=""></a>
  </div>
</template>

<script>
import EnrollBar from './EnrollBar.vue';
import WelcomeComp from './WelcomeComp.vue';
import ClassesComp from './ClassesComp.vue';
import StaffComp from './StaffComp.vue';
import TitleComp from "./TitleComp.vue";
import NewsComp from "./NewsComp.vue";

export default {
name: 'MainComp',
components: {
    EnrollBar,
    WelcomeComp,
    ClassesComp,
    StaffComp,
    TitleComp,
    NewsComp,
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
    ],
    postcards: [
      {
        date: 'October 03, 2014',
        title: 'Drawing and Painting Lessons',
        text: 'Magna est consectetur interdum modest dictum. Curabitur est faucibus, malesuada esttincidut etos et mauris, nunc a libero govum est cuprum.',
        image: 'blog_09-525x315.jpg',
        number: '42',
        productor: 'Anna Brown',
        section: 'Events, Fun'
      },
      {
        date: 'October 03, 2014',
        title: 'Fall Parents Meeting Day',
        text: 'Magna est consectetur interdum modest dictum. Curabitur est faucibus, malesuada esttincidut etos et mauris, nunc a libero govum est cuprum.',
        image: 'blog_10-525x315.jpg',
        number: '19',
        productor: 'Anna Brown',
        section: 'Dance, Education'
      },
      {
        date: 'September 20, 2014',
        title: 'Birthday in Kindergarten',
        text: 'Magna est consectetur interdum modest dictum. Curabitur est faucibus, malesuada esttincidut etos et mauris, nunc a libero govum est cuprum.',
        image: 'blog_08-525x315.jpg',
        number: '22',
        productor: 'Anna Brown',
        section: 'Games, General'
      },
    ]
  }
}
}
</script>

<style lang="scss" scoped>
.container-80 {
  width: 80%;
  margin: auto;
}
</style>