<template>
  <div>
    <div class="text-center m-4">
        <h1>Welcome to Fable</h1>
        <p>Fable daycare, preschool, and kindergarten</p>
        <div>
            <img src="../assets/img/images/header_divider.png" alt="waves">
        </div>
    </div>
    
    <div>
        <div v-for="(elem, index) in welcomeData" :key="index" class="w-card">
            <img :src="require(`../assets/img/images/${elem.image}`)" alt="none">
            <h3> {{elem.title}} </h3>
            <p> {{elem.notes}} </p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
name: 'WelcomeComp',
data() {
    return {
        welcomeData : [
            {
              image: 'schoolbag_alt.png',
              title: 'Morbi Etos',
              notes: 'Praesaent interdum est gravida vehicula est node maecenas loareet morbi a dosis luctus novum est praesent.',
            },
            {
              image: 'stroller_alt.png',
              title: 'Congue Gravida',
              notes: 'Elipsis magna a terminal nulla elementum morbi elite forte maecenas est magna etos interdum vitae est.',
            },
            {
              image: 'globe_alt.png',
              title: 'Maecenas Node',
              notes: 'Praesaent interdum est gravida vehicula est node maecenas loareet morbi a dosis luctus novum est praesent.',
            },
            {
              image: 'bell_alt.png',
              title: 'Praesent Morbi',
              notes: 'Praesaent interdum est gravida vehicula est node maecenas loareet morbi a dosis luctus novum est praesent.',
            },
        ]
    }
}
}
</script>

<style lang="scss" scoped>

</style>