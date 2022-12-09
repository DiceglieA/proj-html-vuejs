<template>
    <div class="container">
        <nav class="row justify-content-between m-auto">
            <div class="col-3">
                <img class="w-50" src="../assets/img/images/logo.png" alt="logo-fable">
            </div>
            <ul class="col-6 d-flex align-items-center ">
                <a v-for="(elem, index) in navList" :key="index" @click="navselect(index)" :class="index === activeindex ? 'active' : ''" class="text-center align-items-center mx-1 py-2">
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
        activeindex: 0,
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
},
methods: {
    navselect(index) {
        this.activeindex = index
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
a:hover {
    background-color: #e8e6e7;
    border-bottom: 2px solid #4c4a9b;;
}
.orange {
    background-color: #fe6601;
}
.active {
    background-color: #fe6601;
    color: white;
}

</style>