<template>
  <div class="w-100">
    <div class="mapouter w-100">
      <div class="gmap_canvas">
      <iframe width="100%" height="500" id="gmap_canvas" src="https://maps.google.com/maps?q=2880%20Broadway,%20New%20York&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
      <a href="https://123movies-to.org"></a>
      <br>
      <a href="https://www.embedgooglemap.net">embed google map in html</a>
    </div>
  </div>
  </div>
</template>

<script>
export default {
name: 'MapComp'
}
</script>

<style lang="scss" scoped>
.mapouter{
  position:relative;
  text-align:right;
  height:500px;width:100%;
}
.gmap_canvas {
  overflow: hidden;
  background:none!important; 
  height:500px;width:100%;
  }
</style>