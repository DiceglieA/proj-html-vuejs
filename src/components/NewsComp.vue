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
            <span class="col-6">{{post.productor}}</span>
            <span class="col-6">{{post.section}}</span>
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
    margin: .8em 0;
}
</style>