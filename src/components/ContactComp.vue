<template>
    <div class="container-contact">
       <div class="row text-center">
            <div class="contact-card col-3">
                <div>
                    <img class="my-3" src="../assets/img/images/envelope (1).png" alt="">
                </div>
                <h5>Postal Address</h5>
                <div>
                    <div>Fable Care Center</div>
                    <div>85 Fentiman Ave</div>
                    <div>Ottawa, ON K1S 0T7</div>
                </div>
            </div>
            <div class="contact-card col-3">
                <div>
                    <img class="my-3" src="../assets/img/images/mobile.png" alt="">
                </div>
                <h5>Phone & E-mail</h5>
                <div>
                    <div>Phone: 1-800-64-38</div>
                    <div>Fax: 1-800-64-39</div>
                    <a href="#!">office@fable.com</a>
                </div>
            </div>
            <div class="contact-card col-3">
                <div>
                    <img class="my-3" src="../assets/img/images/clock.png" alt="">
                </div>
                <h5>Business Hours</h5>
                <div>
                    <div>Monday-Friday</div>
                    <div>8.00 am - 5.00 pm</div>
                    <div>Weekend Closed</div>
                </div>
            </div>
            <div class="contact-card col-3">
                <div>
                    <img class="my-3" src="../assets/img/images/document (1).png" alt="">
                </div>
                <h5>Sessions</h5>
                <div>
                    <div>Mornings, 8 am - 12 noon</div>
                    <div>8Afternoons, 1 px - 5 pm</div>
                    <div>Full Day, 8am - 5 pm</div>
                </div>
            </div>
       </div> 
       <form class="row p-4 my-4" action="">
        <div class="row col-6">
            <input class="mb-4 p-1" type="text" placeholder="Your Name *">
            <input class="mb-4 p-1" type="mail" placeholder="Your E-mail *">
            <input class="p-1" type="text" placeholder="Subject">
        </div>
        <div class="col-6">
            <input class="w-100 h-100" type="textarea" placeholder="Your Message *">
        </div>
        <div class="d-flex justify-content-center">
            <button>SEND MESSAGE</button>  
        </div>
       </form>
    </div>
</template>

<script>
export default {
name: 'ContactComp',
}
</script>

<style lang="scss" scoped>
.container-contact {
    width: 80%;
    margin: auto;
}
a{
    text-decoration: underline;
}
h5 {
    color: #4c4a9b;
}

input {
    border: 1px solid rgb(76, 74, 155, 0.2);
}
form {
    button{
        border: none;
        background-color: #fe6601;
        margin-top: 40px;
        padding: 8px 12px;
        color: white;
        font-weight: bolder;
    }
}
</style>