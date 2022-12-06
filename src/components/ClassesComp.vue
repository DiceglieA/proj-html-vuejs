<template>
  <div>
    <div class="text-center m-4">
        <h1>Our Classes</h1>
        <p>Our preschool program has four dedicated classes</p>
        <div>
            <img src="../assets/img/images/header_divider.png" alt="waves">
        </div>
    </div>
    <div class="container">
      <div class="row mt-5 mb-3">
        <h4 class="col-6">
        We provided four classes with nine to twenty children each aged twelve month to five years of age.
        </h4>
        <p class="col-6">
        Praesent arcu gravida vehicula est node maecenas loareet morbi a desis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis. Aenean interdum, nibh vitae sodales, magna ante feugiat elit maecenas.
        </p>
      </div>

         <!-- Creare componente Card nel Refactoring -->

      <div>
        <div class="class-card row col-6">  <!--  Possibile componente -->
          <div class="text-card col-6">
            <div>Little Lambs</div>
            <div>Class name</div>
            <div class="row text-center">
              <div class="col-6">
                <div>12-24</div>
                <div>Month olds</div>
              </div>
              <div class="col-6">
                <div>9</div>
                <div>Class size</div>
              </div>
            </div>
          </div>
          <div class="img-card col-6">
            <img src="" alt="">
            <button> READ MORE &gt;</button>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
name: 'ClassesComp',
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
</style>