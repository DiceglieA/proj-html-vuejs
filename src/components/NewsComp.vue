<template>
  <div>
    <div class="post-card">
        <div class="date">{{post.date}}</div>
        <div class="card-img">
            <img :src="require(`../assets/img/images/${post.image}`)" alt="">
            <div>{{post.number}}</div>
        </div>
        <h4>{{post.title}}</h4>
        <p>{{post.text}}</p>
        <div class="row">
            <div class="col-6 d-flex align-items-center subtitle">
                <img src="../assets/img/images/author.png" alt="">
                <span class="px-4">{{post.productor}}</span>
            </div>
            <div class="col-6 d-flex align-items-center subtitle">
                <img src="../assets/img/images/category.png" alt="">
                <span class="px-4">{{post.section}}</span>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
name: 'NewsComp',
props: {
    post: Object
}
}
</script>

<style lang="scss" scoped>
.new-container {
    width: 80%;
    margin: auto;
}
.post-card {
    margin-top: 2rem;
}
.card-img {
    position: relative;
    img {
        width: 100%;
    }
    div {
        text-align: end;
        padding: 5px 10px;
        background-color: #fe6601;
        position: absolute;
        right: 0;
        bottom: 0;
        color: white;
    }
}
h4 {
    color: #4c4a9b;
    padding: .8em 0;
}
.date {
    margin-bottom: .8em;
}
p {
    font-size: 16px;
    padding: .8em 0;
    border-bottom: 1px solid lightgrey;
}
.subtitle {
    color: grey;
    font-size: 13px;
}
</style>