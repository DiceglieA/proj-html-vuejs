<template>
  <div class="container">
    <div class="en-bar">
        <h1>How to Enroll Your Child to a class?</h1>
        <a href="#!">Learn more &gt;</a>
    </div>
  </div>
</template>

<script>
export default {
name: 'EnrollBar',
}
</script>

<style lang="scss" scoped>
.container {
    background-image: url(../assets/img/images/pattern.png);
    height: 90px;
    width: 100%;
}
.en-bar{
    height: 90px;
    width: 80%;
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
    font-size: 25px;
    padding: 2px 3px;
}
</style>