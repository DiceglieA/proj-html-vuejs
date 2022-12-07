<template>
  <div class="container-staff">
    <div class="row mt-5 mb-3">
      <h4 class="col-6 violet">
      Our staff consists of three theachers and one assistant with experience in early childhood care.
      </h4>
      <p class="col-6">
      Praesent arcu gravida vehicula est node maecenas loareet morbi a desis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis. Aenean interdum, nibh vitae sodales, magna ante feugiat elit maecenas.
      </p>
    </div>
    <CardstaffComp /> <!-- (da ciclare ) -->
    
  </div>
</template>

<script>
import CardstaffComp from './CardstaffComp.vue'
export default {
name: 'StaffComp',
component: {
  CardstaffComp,
},
data() {
  return {
    staff: [
      {
        name: 'Ruth Richie',
        profession: 'Teacher',
        description: 'I have just finisched my studies in Early Childhood Education, and i am also the kid s yoga teacher here at Fable. I enjoy cooking, swimming and bike riding in my free time.',
        social: ['mail.png','facebook.png','pinterest.png',]
      },
      {
        name: 'Katie Willmore',
        profession: 'Assistant Teacher',
        description: 'IMy name is Katie. I grew up and studied in Canada. This is my second year at Fable and love every minute of it,making the children s learning experience fun.',
        social: ['dribbble.png','stumbleupon.png','instagram.png']
      },
      {
        name: 'Angelica Watson',
        profession: 'Lead Teacher',
        description: 'I hold a degree in Early Childhood Education and in advanced English language certificate. I have been a workingk as a kindergarten teacher since 2002.',
        social: ['bing.png','skype.png','linkedin.png']
      },
      {
        name: 'Angela Lynn',
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
</style>