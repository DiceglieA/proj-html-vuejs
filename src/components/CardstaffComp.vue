<template>
  <div>
    <div class="staff-card row mb-5">
      <div class="left col-6">
        <div>
          <img class="w-100" :src="require(`../assets/img/images/${staff.image}`)" alt="">
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
</style>