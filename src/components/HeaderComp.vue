<template>
  <div>
    <NavComp class="nav"/>
    <JumboComp />
  </div>
</template>

<script>
import NavComp from "./NavComp.vue"
import JumboComp from "./JumboComp.vue"

export default {
name: 'HeaderComp',
components: {
  NavComp,
  JumboComp,
}
}
</script>

<style lang="scss" scoped>
.nav {
  width: 80%;
  margin: auto;
}
</style>