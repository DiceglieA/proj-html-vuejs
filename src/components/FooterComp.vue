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
                    <li>OCTOBER 2014 (2)</li>
                    <li>SEPTEMBER 2014 (2)</li>
                    <li>AUGUST 2014 (2)</li>
                    <li>JULY 2014 (2)</li>
                    <li>JUNE 2014 (2)</li>
                    <li>MAY 2014 (1)</li>
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
            <div class="col-3"></div>
        </div>
    </section>
    <section class="social">

    </section>
  </div>
</template>

<script>
export default {

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
</style>