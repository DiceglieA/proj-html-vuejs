<template>
  <div>
    <section class="background-violet">
        <div class="row v-container">
            <div class="col-3 px-3">
                <div class="title-section">
                    ABOUT US
                </div>
                <div class="line"></div>
                <p>
                    Elipsis magna a nulla elite forte maecenas est elementum magna etos inderdum movum morbi vehicula morbi.
                </p>
                <div>
                    <img class="w-100" src="../assets/img/images/logo_footer.png" alt="">
                </div>
            </div>
            <div class="col-3 px-3">
                <div class="title-section">
                    ARCHIVES
                </div>
                <div class="line"></div>
                <ul class="p-0 archive">
                    <a href="#!"><li>OCTOBER 2014 (2)</li></a>
                    <a href="#!"><li>SEPTEMBER 2014 (2)</li></a>
                    <a href="#!"><li>AUGUST 2014 (2)</li></a>
                    <a href="#!"><li>JULY 2014 (2)</li></a>
                    <a href="#!"><li>JUNE 2014 (2)</li></a>
                    <a href="#!"><li>MAY 2014 (1)</li></a>
                </ul>
            </div>
            <div class="col-3 px-3 features">
                <div class="title-section">
                    OUR FEATURES
                </div>
                <div class="line"></div>
                <p>
                    Nunc gravida rutrum mauris vehin hasellus ac pretium augue vivamul lacus ligul mattis ac vene:
                </p>
                <ul class="p-0">
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Friendly and welcoming place</span>            
                    </li>
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Science and art classes</span>            
                    </li>
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Positive learning environment</span>            
                    </li>
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Educational field trips</span>            
                    </li>
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Writing and reading classes</span>            
                    </li>
                    <li>
                        <img src="../assets/img/images/style_4_alt.png" alt="thick">
                        <span>Science and art classes</span>            
                    </li>
                </ul>
            </div>

<!-- TODO: emit da maincomp array poste proprs array -->

            <div class="col-3">
                <div class="title-section">
                    RECENT POST
                </div>
                <div class="line"></div>
                <div class="row mb-3">
                    <div class="col-4">
                        <img class="w-100 " src="../assets/img/images/blog_09-150x150.jpg" alt="">
                    </div>
                    <div class="col-8">
                        <div class="title-post">
                            Drawing and Painting Lessons
                        </div>
                        <div>
                            <img src="../assets/img/images/date_footer.png" alt="">
                            <span class="date-post">October 03, 2014</span>
                        </div>
                    </div>
                </div>
                
                <div class="row mb-3">
                    <div class="col-4">
                        <img class="w-100" src="../assets/img/images/blog_10-150x150.jpg" alt="">
                    </div>
                    <div class="col-8">
                        <div class="title-post">
                            Fall Parents Meeting Day
                        </div>
                        <div>
                            <img src="../assets/img/images/date_footer.png" alt="">
                            <span class="date-post">October 03, 2014</span>
                        </div>
                    </div>
                </div>

                <div class="row">
                    <div class="col-4">
                        <img class="w-100" src="../assets/img/images/blog_08-150x150.jpg" alt="">
                    </div>
                    <div class="col-8">
                        <div class="title-post">
                            Birthday in Kindergarten
                        </div>
                        <div>
                            <img src="../assets/img/images/date_footer.png" alt="">
                            <span class="date-post">September 20, 2014</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="social-container">
        <div class="d-flex justify-content-center">
            <div class="social">
                <a href="#!"><img src="../assets/img/images/behance.png" alt=""></a>
            </div>
            <div class="social">
                <a href="#!"><img src="../assets/img/images/dribbble.png" alt=""></a>
            </div>
            <div class="social">
                <a href="#!"><img src="../assets/img/images/envato.png" alt=""></a>
            </div>
            <div class="social">
                <a href="#!"><img src="../assets/img/images/facebook.png" alt=""></a>
            </div>
            <div class="social">
                <a href="#!"><img src="../assets/img/images/twitter.png" alt=""></a>
            </div>
        </div>
        <div class="credit violet">
            &#169; Fable - Children Kindergarten WordPress Theme by QuanticaLabs
        </div>
    </section>
  </div>
</template>

<script>
export default {
name: 'FooterComp',
props: {
    post: Object
}
}
</script>

<style lang="scss" scoped>
.background-violet{
    background-image: url(../assets/img/images/pattern.png);
    color: rgb(255, 255, 255, 0.8);
}
.v-container {
    width: 80%;
    margin: auto;
    padding: 3rem 0 6rem;
}
.title-section {
    font-weight: bolder;
    font-size: 20px;
}
.line {
    border-top: 1px solid rgb(255, 255, 255);
    width: 54px;
    margin-top: 10px;
    margin-bottom: 28px;
}
p {
    font-size: 14px;
}
.archive {
    li {
        font-size: 14px;
        font-weight: bold;
        border: 2px solid rgb(255, 255, 255, 0.2);
        margin: 4px 0;
        padding: 12px;
        color: white;
    }
}
.features {
    li {
        font-size: 13px;
        margin: 10px 0;
    }
    img {
        margin-right: 6px;
    }
}
.title-post {
font-weight: bolder;
font-size: 14px;
}

.date-post {
    font-size: 14px;
    margin-left: 10px;
}
.social {
background-color: #fe6601;
margin: 30px 1px;
}
.credit {
text-align: center;
margin-bottom: 25px;
}
</style>