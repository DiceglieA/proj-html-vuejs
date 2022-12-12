<template>
  <div>
    <!-- <let-it-snow
      v-bind="snowConf"
      :show="show"    
    > -->
      <HeaderComp />
      <MainComp />
      <FooterComp />    
    <!-- </let-it-snow> -->
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue";
import MainComp from "./components/MainComp.vue";
import FooterComp from "./components/FooterComp.vue";

export default {
  name: "App",
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  },
  data () {
    return {
        snowConf: {
            windPower : 1,  
            speed : 3,
            count : 12,
            size : 10,
            opacity : 1,
            images: ['https://raw.githubusercontent.com/bob-chen/let_it_snow/master/demo/snow.png',
                    'https://raw.githubusercontent.com/bob-chen/let_it_snow/master/demo/sock.png',
                    'https://raw.githubusercontent.com/bob-chen/let_it_snow/master/demo/tree.png']
        },
        show: true      
    }
  },
  mounted () {
      this.show = false
    //   setTimeout( () => {
    //       this.show = false
    //   }, 5000)
 
    //   setTimeout( () => {
    //       this.show = true
    //   }, 10000)      
  }  
};
</script>

<style lang="scss">

@import "~bootstrap/scss/bootstrap";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  overflow-x: hidden;
}

ul {
  list-style-type: none;
}
a {
  text-decoration: none;
}
.violet {
    color: #4c4a9b;
}
.bg-violet {
  background-color: #4c4a9b;
}
</style>
