<template>
    <div class="container">
        <nav class="row justify-content-between align-items-center">
            <div class="col-3">
                <img class="w-75" src="../assets/img/images/logo.png" alt="logo-fable">
            </div>
            <ul class="col-6 d-flex align-items-center">
                <li v-for="(elem, index) in navList" :key="index" class="text-center align-items-center mx-1">
                    <img :src="require(`../assets/img/${elem.img}`)">
                    <div>{{elem.name}}</div>
                </li>
            </ul>
        </nav>
    </div>
    
</template>

<script>

export default {
name: 'NavComp',
data() {
    return {
        navList: [
            {
                img: "home.png",
                name: "Home"
            },
            {
                img: "document.png",
                name: "Pages"
            },
            {
                img: "printer.png",
                name: "Blog"
            },
            {
                img: "cart.png",
                name: "Shop"
            },
            {
                img: "lab.png",
                name: "Shortcodes"
            },
            {
                img: "chat.png",
                name: "Support"
            },
            {
                img: "envelope.png",
                name: "Contact"
            },
        ]
    }
}
}
</script>

<style lang="scss" scoped>
nav {
    height: 80px;
}
</style>