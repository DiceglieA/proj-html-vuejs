<template>
  <div>
    <NavComp />
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
</style>