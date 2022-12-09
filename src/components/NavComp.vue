<template>
    <div class="container">
        <nav class="row justify-content-between m-auto">
            <div class="col-3">
                <img class="w-50" src="../assets/img/images/logo.png" alt="logo-fable">
            </div>
            <ul class="col-6 d-flex align-items-center">
                <a v-for="(elem, index) in navList" :key="index" @click="navselect(index)" :class="index === activeindex ? 'active' : ''" class="text-center align-items-center px-2 py-1 d-flex flex-column">
                    <img :src="require(`../assets/img/${elem.image}`)" class="p-2" :class="index === activeindex ? 'hidden' : 'block'">
                    <img :src="require(`../assets/img/${elem.images}`)" class="p-2" :class="index === activeindex ? 'block' : 'hidden'">
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
                images: "home-2.png",
                name: "Home"
            },
            {
                image: "document.png",
                images: "document-2.png",
                name: "Pages"
            },
            {
                image: "printer.png",
                images: "printer-2.png",
                name: "Blog"
            },
            {
                image: "cart.png",
                images: "cart-2.png",
                name: "Shop"
            },
            {
                image: "lab.png",
                images: "lab-2.png",
                name: "Shortcodes"
            },
            {
                image: "chat.png",
                images: "chat-2.png",
                name: "Support"
            },
            {
                image: "envelope.png",
                images: "envelope-2.png",
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
    height: 90px;
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
.hidden {
    display: none;
}
.block {
    display: block;
}

</style>