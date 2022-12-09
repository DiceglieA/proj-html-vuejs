<template>
  <div>
    <section class="w-container">  <!-- <! Sezione 1 !> -->
        <div class="row">
            <div v-for="(elem, index) in welcomeData" :key="index" class="w-card col-3 text-center">
                <div class="w-100 mb-3">
                    <img :src="require(`../assets/img/images/${elem.image}`)" alt="none" class="img-card" :class="((index % 2) == 0) ? 'orange' : 'bg-violet' ">
                </div>
                <h3 class="my-3 violet"> {{elem.title}} </h3>
                <p> {{elem.notes}} </p>
            </div>
        </div>
    </section>
    
    <section class="bg-section">  <!-- <! Sezione 2 !> -->
        <div class="w-container row py-5 px-1">
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
            <div class="right col-6 p-0">   <!-- Parte destra -->
                <div>
                    <div class="img-big">
                        <div class="p-0">
                            <img class="w-100" src="../assets/img/images/gallery_01-690x506.jpg" alt="">
                        </div>
                        <div class="d-flex justify-content-between btn-stripe">
                            <div class="btn b-left" @click="changeSlide(-1)">&lt;</div>
                            <div class="btn b-right" @click="changeSlide(1)">&gt;</div>
                        </div>
                    </div>
                    <div class="thumbnails row" >
                        <div class="img-small col-4 gutter" v-for="(elem, index) in carousel" :key="index" @click="setactivendex(index)" :class="{active: index === activeindex}">
                            <img class="w-100 mb-1" :src="require(`../assets/img/images/${elem.image}`)" alt="">
                        </div>
                    </div>
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

    <section class="bg-kids">   <!-- sezione 3 -->
        <div class="row w-container">
            <div v-for="(elem, index) in statsData" :key="index" class="data-card text-center col-3">
                <div class="n-card"> {{elem.number}} </div>
                <div class="title-card"> {{elem.name}} </div>
                <p class="descript-card"> {{elem.description}} </p>
            </div>
        </div>
    </section>
  </div>
</template>

<script>

export default {
name: 'WelcomeComp',
data() {
    return {
        activeindex : 0,
        direction : 1,
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
        ],
        carousel : [
            {
                image:'gallery_07-690x506.jpg',
            },
            {
                image:'gallery_01-690x506.jpg',
            },
            {
                image:'gallery_08-690x506.jpg',
            }
        ],
        statsData : [
            {
                number: '507',
                name: 'Our Pupils',
                description: 'Pulvinar forte maestro mode terminal est elipsis prism',
            },
            {
                number: '235',
                name: 'Teaching Hours',
                description: 'Elipsis morbi nulla a metro interdum vitae elite',
            },
            {
                number: '100%',
                name: 'Satisfied Parents',
                description: 'Elementum pulvinar detos diaspis blandit.',
            },
            {
                number: '1050',
                name: 'Meals Per Year',
                description: 'Pulvinar forte maestro mode terminal est elipsis prism',
            },
        ]
    }
},
methods: {
    setactiveindex(index) {
			this.activeindex = index;
		},
    slider(direction) {
			if (direction > 0) {
				this.activeindex++;
				if (this.activeindex === this.carousel.length) {
					this.activeindex = 0;
				}
			} else {
				if (this.activeindex === 0) {
					this.activeindex = this.carousel.length;
				}
				this.activeindex--;
			}
		},
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
.bg-violet {
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
.bg-kids {
    background-image: url('../assets/img/images/parallax_01.jpg');
    background-size: cover;
    background-position: center;
    height: 280px;
    color: white;
}
.data-card {
    margin-top: 50px;
}
.n-card {
    clip-path: circle();
    border: 2px solid white;
    padding: 20px;
    font-size: 30px;
}
.title-card {
    font-weight: bolder;
    margin: 10px;
}
.descript-card {
    font-size: 12px;
    padding: 0 20px;
}

.img-big {
    position: relative;
}
.btn {
    background-color: #fe6601;
    color: white;
    width: 40px;
    height: 40px;
    border-radius: 0;
}
.b-left {
    position: absolute;
    left: 0;
    top: 45%;
}
.b-right {
    position: absolute;
    right: 0;
    top: 45%;
}
.thumbnails {
    padding: 12px 6px;
}
.gutter{
    padding: 0 6px;
}
.active {
    border-bottom: 2px solid #fe6601;
}
</style>