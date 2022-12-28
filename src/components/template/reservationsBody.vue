<template>
    <div class="reservations" id="reservations">
        <div class="container"> 
            <div class="row justify-content-md-center text-center">
                <div class="col-lg-3" id="disappearingBlock">
                    <img src="../../../public/image/ReservImage1.png" alt="">
                </div>
                <div class="col-lg-3" id="disappearingBlock">
                    <img src="../../../public/image/ReservImg2.png" alt="">
                </div>
                <div class="col-6">
                    <div class="row justify-content-md-center text-center">
                        <div class="col-12">
                            <h3>Just the right food</h3>
                        </div>
                        <div class="col-12" id="disappearingBlock">
                            <h6>If you've been to one of our restaurants,you've seen-and
                                <br>tasted - what keeps our customers coming back for more.
                                <br>Perfect materials and freshly baked food.
                                <br>
                                <br>Delicious Lambda cakes,muffins, andgourmet coffes make
                                <br>us hard to resist! Stop in today and check us out! Perfect
                                <br>materials and freshly baked food.
                            </h6>
                        </div>
                        <div class="col-12">
                            <form class="row g-3 text-start">
                                <div class="col-md-6">
                                    <label for="inputName" class="form-label">Your name</label>
                                    <input type="text" class="form-control" id="inputName" placeholder="name">
                                </div>
                                <div class="col-md-6">
                                    <label for="inputEmail" class="form-label">Your email</label>
                                    <input type="email" class="form-control" id="inputEmail" placeholder="e-mail">
                                </div>
                                <div class="col-md-6">
                                    <label for="inputPhone" class="form-label">Your phone number</label>
                                    <input type="tel" class="form-control" id="inputPhone" pattern="\(\d\d\d\) ?\d\d\d-\d\d-\d\d" placeholder="(+375 ##) ###-##-##">
                                </div>
                                    <div class="col-md-6">
                                    <label for="inputEvent" class="form-label">Desired event date</label>
                                <input type="date" class="form-control" id="inputEvent">
                                </div>
                            </form>
                        </div>
                        <div class="row headerButtons justify-content-center gy-5">
                            <a id="bookNow" href="#" class="btn btn-success" @click="DialogShow">BOOK NOW!</a>
                            <MyDialog v-model:show="DialogVisible">
                                <form>
                                    <h5>Thanks!</h5>
                                    <h6>The table is reserved! We'll call you back.</h6>
                                </form>
                            </MyDialog>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<!-- 
rgb(63, 52, 52)
#ffc107 -->

<style scoped>
h3, label{
    color: #ffc107;
}
h6{
    color:rgb(63, 52, 52);
}
.reservations {
    height: 90vh;
    display: flex;
    align-items: center;
}
#bookNow{
    color:white;
    background-color: #ffc107;
    border: none;
    opacity: 100%;
    width: 200px ;
    height:50px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    border-radius: 0em;
}
#bookNow:hover{
    color:white;
    border: none;
    opacity: 100%;
    background-color:#0d6efd;
    text-decoration: none;
}
</style>
<script>
import { ref } from "vue";
export default {
    name: "reservationsBody",
    setup() {
        const DialogVisible = ref(false);
        const DialogShow = (e) => {
            e.preventDefault();
            console.log("test");
            DialogVisible.value = true;
        }
            return {
                DialogVisible,
                DialogShow
            }
        }
    }
</script>