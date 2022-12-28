<template>
    <section class="reviews" id="reviews">
        <div class="container text-white align-items-center justify-content-md-center">
            <div class="row reviewsText">
                <div class="col reviews-cover text-center align-self-center">
                    <div class="row ing-cover text-center">
                        <div class="col-12">
                            <h2>Guest Reviews</h2>
                        </div>
                        <div class="col-12 ">
                            <img src="../../../public/image/Divider.png"  id="divider" alt="">
                        </div>
                        <div class="col-12">
                            <h4>If you've been too one of our restaurants,you've seen - 
                                <br>and tasted - what keeps our customers coming back for
                                <br>more. Perfect materials and freshly baked food,
                                <br>delisious Lambda cakes, muffins, and gourmet coffees
                                <br>make us hard to resist! Stop in today  and chech us out!
                            </h4>
                        </div>
                        <div class="col-12">
                            -food inc, New York
                        </div>
                    </div>
                </div>
            </div>
            <div class="row header-buttons align-items-end justify-content-md-center pt-40 ">
                <div class=" header-but col-lg-4 col-sm-12 text-center text-center text-uppercase ">
                    <a href="#" @click="DialogShow" class="button">Leave a reviews</a>
                    <MyDialog v-model:show="DialogVisible">
                        <form>
                            <h6>Leave your revievs</h6>
                            <div class="mb-9">
                                <textarea></textarea>
                            </div>
                            <button type="submit" class="btn btn-primary">Save</button>
                        </form>
                    </MyDialog>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
    h6{
        color: rgb(63, 52, 52);
    }
    .reviewsText{
        padding-top: 80px;
    }
    .header-buttons{
        padding-top: 90px;
    }
    .header-but{
        display: flex;
        justify-content: space-around;
    }
    .button{
        color:white;
        background-color: black;
        border: 1px solid white;
        width: 200px ;
        height:50px;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: none;
        opacity: 60%;
    }
    .button:hover{
        color:white;
        border: 1px solid white;
        background-color:#0d6efd;
        text-decoration: none;
        opacity: 100%;
    }
#divider{
    height: 35px;
}
.reviews{
    height: 90vh;
}
</style>
<script>
import { ref } from "vue";
export default {
    name: "homeTop",
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