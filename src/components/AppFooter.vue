<script >

    export default{
        name:"AppFooter",
        data(){
            return{

            }
        }
    }
</script>

<template>
    <section>
        <div class="container">

            <div class="botton">
                SIGN-UP NOW!
            </div>

            <div class="social">
                <h4>FOLLOW US</h4>

                <div class="social-link">
                    <a href="#">
                        <img src="../assets/images/footer-facebook.png" alt="">
                    </a>
                </div>
                <div class="social-link">
                    <a href="#">
                        <img src="../assets/images/footer-twitter.png" alt="">
                    </a>
                </div>
                <div class="social-link">
                    <a href="#">
                        <img src="../assets/images/footer-youtube.png" alt="">
                    </a>
                </div>
                <div class="social-link">
                    <a href="#">
                        <img src="../assets/images/footer-pinterest.png" alt="">
                    </a>
                </div>
                <div class="social-link">
                    <a href="#">
                        <img src="../assets/images/footer-periscope.png" alt="">
                    </a>
                </div>
            </div>
        </div>

        <div class="riempimento-footer">
        </div>
    </section>
    
  
</template>
  
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
    
section {
    background-color: #303030;
    height: 100px;
}
.container {
    height: 100%;
    @include between();

    .botton {
        color: $primary;
        width: fit-content;
        padding: 15px;
        border: solid 2px #0282f9;
    }

    .social {
        @include between();
        gap: 20px;
    }

    h4 {
        color: #0282f9;
    }
    .social-link {
        width: 40px;
        height: 40px;
    }
}
.riempimento-footer {
    background-color: #222222;
    height: 100%;
}


</style>