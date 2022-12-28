<template>
    <div>
        <header>
            <div class="container-fluid">
                <div class="row header-nav align-items-center">
                    <div class="col-4 text-center">
                        <h1 class="text-white">LAMBDA</h1>
                    </div>
                    <div class="col-8">
                        <div class="row nav align-items-center">
                            <div class="col-xl-2 col-sm-12">
                                <router-link to="/" class="nav text-white">
                                    <h4>Home</h4>
                                </router-link>
                                <router-view/>
                            </div>
                            <div class="col-xl-2 col-sm-12">
                                <a href="/#about" class="nav text-white">
                                    <h4>About</h4>
                                </a> 
                            </div>
                            <div class="col-xl-2 col-sm-12">
                                <a href="/#ingredients" class="nav text-white">
                                    <h4>Ingredients</h4>
                                </a> 
                            </div>
                            <div class="col-xl-2 col-sm-12">
                                <a href="/#menu" class="nav text-white">
                                    <h4>Menu</h4>
                                </a> 
                            </div>
                            <div class="col-xl-2 col-sm-12">
                                <a href="/#reviews" class="nav text-white">
                                    <h4>Reviews</h4>
                                </a> 
                            </div>
                            <div class="col-xl-2 col-sm-12" title="Log in to your personal account">
                                <a href="#" @click="DialogShow" class="nav text-white">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-person" viewBox="0 0 16 16">
                                        <path d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z"/>
                                    </svg>
                                </a>
                                <MyDialog v-model:show="DialogVisible">
                                    <form class="row g-3">
                                        <div class="col-md-4">
                                            <label for="validationDefault01" class="form-label">Name</label>
                                            <input type="text" class="form-control" id="validationDefault01" value="Anastasiya" required>
                                        </div>
                                        <div class="col-md-4">
                                            <label for="validationDefault02" class="form-label">Surname</label>
                                            <input type="text" class="form-control" id="validationDefault02" value="Kotovich" required>
                                        </div>
                                        <div class="col-md-4">
                                            <label for="validationDefaultUsername" class="form-label">Username</label>
                                            <div class="input-group">
                                            <span class="input-group-text" id="inputGroupPrepend2">@</span>
                                            <input type="text" class="form-control" id="validationDefaultUsername"  aria-describedby="inputGroupPrepend2" required>
                                            </div>
                                        </div>
                                        <div class="col-md-6">
                                            <label for="validationDefault03" class="form-label">City</label>
                                            <select class="form-select" id="validationDefault03" required>
                                                <option selected disabled value="">choose</option>
                                            <option>Minsk</option>
                                            <option>another city</option>
                                            </select>
                                        </div>
                                        <div class="col-md-3">
                                            <label for="validationDefault04" class="form-label">Age</label>
                                            <select class="form-select" id="validationDefault04" required>
                                            <option selected disabled value="">choose</option>
                                            <option>I am not yet 18</option>
                                            <option>I already have 18</option>
                                            </select>
                                        </div>
                                        <div class="col-md-3">
                                            <label for="validationDefault05" class="form-label">Password</label>
                                            <input type="password" class="form-control" id="validationDefault05" required>
                                        </div>
                                        <div class="col-12">
                                            <div class="form-check">
                                            <input class="form-check-input" type="checkbox" value="" id="invalidCheck2" required>
                                            <label class="form-check-label" for="invalidCheck2">
                                                Accept the terms and agreements
                                            </label>
                                            </div>
                                        </div>
                                        <div class="col-12">
                                            <button class="btn btn-primary" type="submit">Submit form</button>
                                        </div>
                                    </form>
                                    <!-- <form>
                                        <div class="mb-3">
                                            <label for="exampleInputEmail1" class="form-label">Email address</label>
                                            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
                                            <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
                                        </div>
                                        <div class="mb-3">
                                            <label for="exampleInputPassword1" class="form-label">Password</label>
                                            <input type="password" class="form-control" id="exampleInputPassword1">
                                        </div>
                                        <button type="submit" class="btn btn-primary">Submit</button>
                                    </form> -->
                                </MyDialog>
                            </div>
                        </div> 
                    </div>
                </div>
                <div class="row header-text text-center font-weight-bold text-white">
                    <div class="col-12">
                        <p class="h1"><strong>the right iingredients
                            <br>for the right food
                        </strong></p>
                    </div>
                </div> 
                <div class="row header-divider">
                    <div class="col-12">
                        <img src="../../../public/image/Divider.png" class="rounded mx-auto d-block" alt="">
                    </div>
                </div>
                <div class="row header-buttons">
                    <div class="col-lg-4 col-sm-0"></div>
                    <div class=" header-but col-lg-4 col-sm-12 text-center text-center text-uppercase">
                        <a href="/#reservations" class="button">BOOK A TABLE</a>
                        <a href="/menu" class="button">SEE THE MENU</a>
                    </div>
                    <div class="col-lg-4 col-sm-0">
                    </div>
                </div>
            </div>
        </header>
    </div>
</template>
<style scoped>
    a{
        text-decoration: none;
    }
    a:hover{
        text-decoration: underline;
    }
    /* .nav text-white:hover{
        color: #0d6efd;
    } */
    svg{
        height: 30px;
        width: 30px;
    }
    .dialog_content{
        z-index: 100;
    }
    .header-but{
        display: flex;
        justify-content: space-around;
    }
    .button{
        color:white;
        background-color: black;
        border: 1px solid white;
        opacity: 50%;
        width: 200px ;
        height:50px;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: none;
    }
    .button:hover{
        color:white;
        border: 1px solid white;
        opacity: 100%;
        background-color:#0d6efd;
        text-decoration: none;
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