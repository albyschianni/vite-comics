<script >

    export default{
        name:"AppMiddle",
        data(){
            return{

            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <div class="assets">
                <a href="#">
                    
                    <div>
                        <img src="../assets/images/buy-comics-digital-comics.png" alt="">
                    </div>

                    <span>DIGITAL COMICS</span>
                </a>
            </div>
            <div class="assets">
                <a href="#">
                    
                    <div>
                        <img src="../assets/images/buy-comics-merchandise.png" alt="">
                    </div>

                    <span>DC MERCHANDISE </span>
                </a>
            </div>
            <div class="assets">
                <a href="#">
                    
                    <div>
                        <img src="../assets/images/buy-comics-subscriptions.png" alt="">
                    </div>

                    <span>SUBSCRIPTION</span>
                </a>
            </div>
            <div class="assets">
                <a href="#">
                    
                    <div>
                        <img src="../assets/images/buy-comics-shop-locator.png" alt="">
                    </div>

                    <span>COMICS SHOP LOCATOR</span>
                </a>
            </div>
            <div class="assets">
                <a href="#">
                    
                    <div>
                        <img src="../assets/images/buy-dc-power-visa.svg" alt="">
                    </div>

                    <span>DC POWER VISA</span>
                </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    background-color: #0282f9;
    color: white;
    height: 150px;
}
.container {
    height: 100%;
    @include between();
    gap: 20px;
}

.assets {
    width: calc((100% - 20px) / 5);

    a {
        color: white;
        height: 100px;
        font-size: 13px;
        text-decoration: none;
        @include center();
    }
        div{
            width: 60px;
            height: 60px;
            margin-right: 10px;
            display: flex;
            align-items: center;
        }
}

</style>
