<template>
  <div>
    <div class="container-staff">
      <div class="row mt-5 mb-3">
        <h4 class="col-6 violet">
        Our staff consists of three theachers and one assistant with experience in early childhood care.
        </h4>
        <p class="col-6">
        Praesent arcu gravida vehicula est node maecenas loareet morbi a desis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis. Aenean interdum, nibh vitae sodales, magna ante feugiat elit maecenas.
        </p>
      </div>
      <div class="row mb-5">
         <CardstaffComp v-for="(elem, index) in staff" :key="index" :staff="staff[index]" class="col-6"/>
      </div>
      <!-- (da ciclare )TODO:  --> 
    </div>
    <div class="bg-kids text-center d-flex flex-column justify-content-center">
      <div>
        <div class="container-quote">
          <img src="../assets/img/images/quote_alt.png" alt="quotes">
        </div>
      </div>
      <div class="text w-75 mx-auto mt-5 mb-4">
        Fable Kindergarten is a great place for my daughter to start her schooling experience. It's welcoming and safe and my daughter loves being there.
      </div>
      <div class="line mx-auto mb-4" />
      <div>
        Joe R. Hamblen
      </div>
    </div>
  </div>
</template>

<script>
import CardstaffComp from './CardstaffComp.vue'

export default {
name: 'StaffComp',
components: {
  CardstaffComp,
},
data() {
  return {
    staff: [
      {
        name: 'Ruth Richie',
        image: 'team_04.jpg',
        profession: 'Teacher',
        description: 'I have just finisched my studies in Early Childhood Education, and i am also the kid s yoga teacher here at Fable. I enjoy cooking, swimming and bike riding in my free time.',
        social: ['mail.png','facebook.png','pinterest.png',]
      },
      {
        name: 'Katie Willmore',
        image: 'team_03.jpg',
        profession: 'Assistant Teacher',
        description: 'IMy name is Katie. I grew up and studied in Canada. This is my second year at Fable and love every minute of it,making the children s learning experience fun.',
        social: ['dribbble.png','stumbleupon.png','instagram.png']
      },
      {
        name: 'Angelica Watson',
        image: 'team_02.jpg',
        profession: 'Lead Teacher',
        description: 'I hold a degree in Early Childhood Education and in advanced English language certificate. I have been a workingk as a kindergarten teacher since 2002.',
        social: ['bing.png','skype.png','linkedin.png']
      },
      {
        name: 'Angela Lynn',
        image: 'team_01.jpg',
        profession: 'Teacher',
        description: 'I have completed a Graduate Diploma in Early Childhood teaching. I have worked with children aged from six weeks to eight years. This is my second year at Fable.',
        social: ['youtube.png','twitter.png','googleplus.png']
      },
    ]
  }
}
}
</script>

<style lang="scss" scoped>
.container-staff {
  width: 80%;
  margin: auto;
}
.bg-kids {
  background-image: url(../assets/img/images/parallax_02.jpg);
  background-size: cover;
  background-position: center;
  height: 400px;
  color: white;

  img {
    width: 60px;
    clip-path: circle();
    border: 2px solid white;
    background-color: transparent;
    border-radius: 50%;
    padding: 10px;
    
    // TODO: fare cerchio
  }

  .text {
    font-size: 20px;
  }

  .line{
    width: 50px;
    border-top: 2px solid white;
  }
}
</style>