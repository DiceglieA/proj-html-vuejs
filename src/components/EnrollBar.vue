<template>
  <div class="container-bar">
    <div class="en-bar">
        <h1>{{datibars.title}}</h1>
        <a href="#!">{{datibars.button}} &gt;</a>
    </div>
  </div>
</template>

<script>
export default {
name: 'EnrollBar',
props: {
  datibars: Object
}
}
</script>

<style lang="scss" scoped>
.container-bar {
    background-image: url(../assets/img/images/pattern.png);
    height: 90px;
    background-size: cover;
}
.en-bar{
    width: 80%;
    height: 90px;
    margin: auto;    
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: white;
}
a {
    text-decoration: none;
    color: white;
    border: 2px solid white;
    font-size: 18px;
    padding: 5px 15px;
}
a:hover {
  background-color: white;
  color: #4c4a9b;
}
</style>