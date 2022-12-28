<template>    
    <section class="menu" id="menu">
        <div class="container overflow-hidden">
            <div class="row menuEat gy-5">
                <div class="col-lg-6" id="disappearingBlock">
                    <div class="p-3 border bg-light">
                        <div class="row justify-content-center">
                            <div class="col-4">
                                <h3>Salads</h3>
                            </div>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6" id="disappearingBlock">
                    <div class="p-3 border bg-light">
                        <div class="row justify-content-center">
                            <div class="col-4">
                                <h3>Soups</h3>
                            </div>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6" id="disappearingBlock">
                    <div class="p-3 border bg-light">
                        <div class="row justify-content-center">
                            <div class="col-4">
                                <h3>Desserts</h3>
                            </div>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="p-3 border bg-light">
                        <div class="row justify-content-center">
                            <div class="col-4">
                                <h3>Snacks</h3>
                            </div>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                        <div class="row justify-content-between namePrice">
                            <div class="col-3">
                                <h6>Olive Speshial</h6>
                            </div>
                            <div class="col-1">2,65$</div>
                        </div>
                        <div>
                            <h>Classic salad with vegetables and sausage</h>
                        </div>
                    </div>
                </div>            
                <div class="row menuButtons justify-content-center gy-5">
                    <div class=" menuBut col-lg-4 col-sm-12 text-center text-uppercase">
                    <a href="/menu" class="button">SEE MENU</a>
                    </div>
                </div>
            </div>
        </div>
    </section> 
</template>
<style scoped>
    .namePrice{
        border-bottom: 0.5px solid  #ffc107;
        padding-top: 15px;
    }
    h{
        color: rgb(63, 52, 52);
    }
    .menuEat{
      color: #ffc107;   
    }
    .menu{
    height: 90vh;
    display: flex;
    align-items: center;
    }
    .menuBut{
        display: flex;
        justify-content: space-around;
    }
    .button{
        color:white;
        background-color: #ffc107;
        border: 1px solid white;
        opacity: 90%;
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



