<template>
  <div>
    <div class="staff-card row mb-5">
      <div class="left col-6">
        <div class="img-plus">
          <img class="w-100" :src="require(`../assets/img/images/${staff.image}`)" alt="">
          <div class="hover-plus text-center">+</div>
        </div>
        <div class="text-center py-2 hover-violet">
          <div class="violet">{{staff.name}}</div>
          <div>{{staff.profession}}</div>
        </div>
      </div>
      <div class="right col-6">
        <div class="my-4 quotes">
          <img src="../assets/img/images/quote.png" alt="">
        </div>
        <p>{{staff.description}}</p>
        <div class="d-flex">
          <div class="social">
            <img :src="require(`../assets/img/images/${staff.social[0]}`)" alt="">
          </div>
          <div class="social">
            <img :src="require(`../assets/img/images/${staff.social[1]}`)" alt="">
          </div>
          <div class="social">
            <img :src="require(`../assets/img/images/${staff.social[2]}`)" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
name: 'CardstaffComp',
props: {
    staff: Object
}
}
</script>

<style lang="scss" scoped>
.quotes {
  border: 2px solid #fe6601;
  padding: 10px 20px;
  width: 50%;
  text-align: end;
  margin-left: -50px;
}
.social {
  background-color: #fe6601;
  margin-right: 4px;
}
.left:hover .hover-violet{
  background-color: #e8e6e7;
}
.img-plus {
  position: relative;
}
.hover-plus {
  background-color: rgb(76, 74, 155, 0.2);
  width: 60px;
  height: 60px;
  border-radius: 50%;
  color: white;
  position: absolute;
  top: 40%;
  left: 40%;
  z-index: 10;
  font-size: 35px;
  display: none;
}
.left:hover .hover-plus {
  display: block;
}
</style>