<template>
  <div>
    <div class="text-center m-4">
        <h1 class="violet">{{datititle.title}}</h1>
        <p>{{datititle.subtitle}}</p>
        <div>
          <img :src="require(`../assets/img/images/${datititle.image}`)">
        </div>
    </div>
  </div>
</template>

<script>
export default {
name: 'TitleComp',
props: {
  datititle: Object
}
}
</script>

<style lang="scss" scoped>

</style>