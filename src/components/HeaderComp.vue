<template>
  <div>
    <NavComp class="nav"/>
    <JumboComp />
    <EnrollBar />
  </div>
</template>

<script>
import NavComp from "./NavComp.vue"
import JumboComp from "./JumboComp.vue"
import EnrollBar from './EnrollBar.vue'
export default {
name: 'HeaderComp',
components: {
  NavComp,
  JumboComp,
  EnrollBar,
}
}
</script>

<style lang="scss" scoped>
.nav {
  width: 80%;
  margin: auto;
}
</style>