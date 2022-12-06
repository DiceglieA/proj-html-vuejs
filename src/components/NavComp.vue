<template>
    <div class="container">
        <nav class="row justify-content-between m-auto">
            <div class="col-3">
                <img class="w-50" src="../assets/img/images/logo.png" alt="logo-fable">
            </div>
            <ul class="col-6 d-flex align-items-center ">
                <a v-for="(elem, index) in navList" :key="index" class="text-center align-items-center mx-1 py-2">
                    <img :src="require(`../assets/img/${elem.image}`)" class="p-2">
                    <div>{{elem.name}}</div>
                </a>
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
                image: "home.png",
                name: "Home"
            },
            {
                image: "document.png",
                name: "Pages"
            },
            {
                image: "printer.png",
                name: "Blog"
            },
            {
                image: "cart.png",
                name: "Shop"
            },
            {
                image: "lab.png",
                name: "Shortcodes"
            },
            {
                image: "chat.png",
                name: "Support"
            },
            {
                image: "envelope.png",
                name: "Contact"
            },
        ]
    }
}
}
</script>

<style lang="scss" scoped>
.container {
    width: 80%;
}
nav {
    height: 90px;
}
a {
    text-decoration: none;
    cursor: pointer;
    color: #594e9e;
}

</style>