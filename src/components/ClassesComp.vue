<template>
  <div>
    <div class="container">
      <div class="row mt-5 mb-3">
        <h4 class="col-6 violet">
        We provided four classes with nine to twenty children each aged twelve month to five years of age.
        </h4>
        <p class="col-6">
        Praesent arcu gravida vehicula est node maecenas loareet morbi a desis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis. Aenean interdum, nibh vitae sodales, magna ante feugiat elit maecenas.
        </p>
      </div>

         <!-- Creare componente Card nel Refactoring -->

      <div class="row mb-5">
        <div v-for="(elem, index) in classData" :key="index" class="class-card row col-6 m-auto">  <!--  Possibile componente -->
          <div class="text-card p-3 col-6">
            <div>{{elem.name}}</div>
            <div class="sizing">Class name</div>
            <div class="row text-center sizing">
              <div class="col-6 mt-5">
                <div>{{elem.age}}</div>
                <div>{{elem.description}} olds</div>
              </div>
              <div class="col-6 mt-5">
                <div>{{elem.size}}</div>
                <div>Class size</div>
              </div>
            </div>
          </div>
          <div class="img-card col-6 p-0">
            <img :src="require(`../assets/img/images/${elem.image}`)" alt="">
            <button> READ MORE &gt;</button>
          </div>
        </div>
      </div>

    </div>
    <!-- componente sfondo viola -->
    <div>
      <AchievementComp />
    </div>
    <!-- componente immagini fascia(forse) -->
    <div class="row">
      <div class="col-3 p-0">
        <img class="w-100" src="../assets/img/images/gallery_01-690x506.jpg" alt="">
      </div>
      <div class="col-3 p-0">
        <img class="w-100" src="../assets/img/images/gallery_02-690x506.jpg" alt="">
      </div>
      <div class="col-3 p-0">
        <img class="w-100" src="../assets/img/images/gallery_03-690x506.jpg" alt="">
      </div>
      <div class="col-3 p-0">
        <img class="w-100" src="../assets/img/images/gallery_04-690x506.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
import AchievementComp from './AchievementComp.vue'
export default {
name: 'ClassesComp',
components: {
  AchievementComp,
},
data() {
  return {
    classData: [
      {
        name:'Little Lambs',
        age: '12-24',
        description: 'Month',
        size:'9',
        image:'class_01-690x506.jpg',
      },
      {
        name:'Bouncy Bears',
        age: '2-3',
        description: 'Year',
        size:'12',
        image:'class_02-690x506.jpg',
      },
      {
        name:'Tenderhearts',
        age: '3-4',
        description: 'Year',
        size:'15',
        image:'class_03-690x506.jpg',
      },
      {
        name:'Shining Stars',
        age: '4-5',
        description: 'Year',
        size:'20',
        image:'class_04-690x506.jpg',
      },
    ]
  }
}
}
</script>

<style lang="scss" scoped>
.container {
  width: 80%;
  margin: auto;
}
.class-card {
  height: 200px;
  padding: 12px;
}
.text-card {
  background-color: #4c4a9b;
  color: white;
}
.sizing {
  font-size: 12px;
}
.img-card{
  position: relative;
  img {
    width: 100%;
  }
  button {
    position: absolute;
    right: 0;
    bottom: 0;
    background-color: #fe6601;
    color: white;
    border: none;
    font-size: 12px;
    padding: 10px;
  }
}

</style>