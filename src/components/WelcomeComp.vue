<template>
  <div class="w-container">
    <div class="text-center m-4">
        <h1>Welcome to Fable</h1>
        <p>Fable daycare, preschool, and kindergarten</p>
        <div>
            <img src="../assets/img/images/header_divider.png" alt="waves">
        </div>
    </div>
    
    <section>  <!-- <! Sezione 1 !> -->
        <div class="row">
            <div v-for="(elem, index) in welcomeData" :key="index" class="w-card col-3 text-center">
                <div class="w-100 mb-3">
                    <img :src="require(`../assets/img/images/${elem.image}`)" alt="none" class="img-card" :class="((index % 2) == 0) ? 'orange' : 'violet' ">
                </div>
                <h3 class="my-3"> {{elem.title}} </h3>
                <p> {{elem.notes}} </p>
            </div>
        </div>
    </section>
    
    <section class="bg-section">  <!-- <! Sezione 2 !> -->
        <div class="row py-5 px-1">
            <div class="left col-6">    <!-- Parte sinistra -->
                <div class="d-flex">
                    <div class="overview orange">
                        Overview
                    </div>
                    <div class="overview mission">
                        Our Mission
                    </div>
                </div>
                <p class="description title">
                    Our philosophy is learning thorugh play as we offer a stimulating environment for children.
                </p>
                <div v-for="(elem, index) in learningData" :key="index" class="d-flex">
                    <div class="col-2 me-3">
                        <img :src="require(`../assets/img/images/${elem.image}`)" alt="none" class="orange img-overview">
                    </div>
                    <div class="pe-4">
                        <h3 class="title"> {{elem.title}} </h3>
                        <p class="p-2"> {{elem.notes}} </p>
                    </div>
                </div>
            </div>
            <!-- carosello -->
            <div class="right col-6">   <!-- Parte destra -->
                <div>

                </div>
                <!-- <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
                    <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="..." class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="..." class="d-block w-100" alt="...">
                    </div>
                    <div class="carousel-item">
                        <img src="..." class="d-block w-100" alt="...">
                    </div>
                    </div>
                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                    </button>
                </div> -->
            </div>
        </div>
    </section>

    <section>   <!-- sezione 3 -->
        <div></div>
    </section>
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
        ],
        learningData : [
            {
                image: 'clock_alt.png',
                title: 'Full Day Session',
                notes: 'Pulvinar est metro ligula blandit maecenas retrum gravida cuprum. Maecenas node estibulum.',
            },
            {
                image: 'diagram_alt.png',
                title: 'Varied Classes',
                notes: 'Pulvinar est metro ligula blandit maecenas retrum gravida cuprum. Maecenas node estibulum.',
            }
        ]
    }
}
}
</script>

<style lang="scss" scoped>
.w-container {
    width: 80%;
    margin: auto;
}
.orange {
    background-color: #fe6601;
}
.violet {
    background-color: #554e95;
}
.img-card {
    clip-path: circle();
    padding: 3rem;
    margin-left: 1.2rem;
}
.w-card {
    padding: 1rem;
}
.bg-section {
    background-color: #e8e6e7;
}

.left {
    .description {
        font-size: 30px;
        margin: 30px 70px 30px 0px;
        line-height: 1.2em;
    }
    
    .overview {
    font-size: 18px;
    padding: .5rem 1.2rem;
    color: white;
    }
    .mission {
        color: grey;
    }
    .img-overview{
        clip-path: circle();
        padding: 1.5rem;
    }
    .title {
        color: #554e95;
    }
}


</style>