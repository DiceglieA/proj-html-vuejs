<template>
  <div class="bg-purple">
    <div class="container">
        <div class="left col-6 py-5">
            <h4 class="mb-4 violet">We have been educating children for over fifteen years. Our goal is to create a place that emgages each child.
            </h4>

            <p class="mb-4">Praesent arcu gravida vehicula est node maecenas loareet morbi a desis luctus. Urna eget lacinia eleifend praesent luctus a arcu quis facilisis venenatis, aenean interdum,</p>

            <ul class="p-0">
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Comprensive reporting on individual achievement</span>            
            </li>
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Educational field trips and school presentations</span>            
            </li>
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Individual attention in a small-class setting</span>            
            </li>
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Learning program with after-school care</span>            
            </li>
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Opportunities to carry out scientific investigations</span>            
            </li>
            <li>
                <img src="../assets/img/images/style_1.png" alt="thick">
                <span>Positive Learning environment for your child</span>            
            </li>
            </ul>
        </div>
        <div class="right row col-6 py-5 text-center">
            <div v-for="(elem, index) in achieveData" :key="index" class="col-6">
                <img :src="require(`../assets/img/images/${elem.image}`)" alt="none" class="img-card mt-2">
                <h5 class="my-3 violet">{{elem.title}}</h5>
                <p>{{elem.subtitle}}</p>
            </div>
        </div>
    </div>
    
  </div>
</template>

<script>
export default {
name: 'AchievementComp',
data() {
    return {
        achieveData: [
            {
                title: 'Learning & Fun',
                subtitle: 'Praesent modea est gravida node vehicula luctus.',
                image: 'toy.png'
            },
            {
                title: 'Healty Meals',
                subtitle: 'Terminal interdum a eleifend maecenas est morbi.',
                image: 'meal.png'
            },
            {
                title: 'Friendly Place',
                subtitle: 'Terminal interdum a eleifend maecenas est morbi.',
                image: 'school.png'
            },
            {
                title: 'Children Safety',
                subtitle: 'Praesent modea est gravida node vehicula luctus.',
                image: 'shield.png'
            }
        ]
    }
}
}
</script>

<style lang="scss" scoped>
.bg-purple {
    background-color: #e8e6e7;
}
.container {
    width: 80%;
    display: flex;
}
.left {
    font-size: 13px;
    line-height: 1.6em;
    li {
        display: flex;
        align-items: center;
    }
    span {
        margin-left: 15px;
    }
    img{
        width: 13px;
    }
}
.right {
    font-size: 12px;
}
.img-card{
    clip-path: circle();
    background-color: white;
    padding: 1rem;
    width: 23%;
}
.violet {
    color: #4c4a9b;
}

</style>