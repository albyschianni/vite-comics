<script>

    export default{
        name:"AppUpFooter",
        data(){
            return{
                menu:[
                    {
                        title:"DC COMICS",
                        links: [
                            {
                                url:"#",
                                text:"Characters"
                            },
                            {
                                url:"#",
                                text:"Comics"
                            },
                            {
                                url:"#",
                                text:"Movies"
                            },
                            {
                                url:"#",
                                text:"Tv"
                            },
                            {
                                url:"#",
                                text:"Games"
                            },
                            {
                                url:"#",
                                text:"Videos"
                            },
                            {
                                url:"#",
                                text:"News"
                            },
                        ]
                    },
                    {
                        title:"SHOP",
                        links:[
                            {
                                url:"#",
                                text:"Shop DC"
                            },
                            {
                                url:"#",
                                text:"Shop DC Collectibles"
                            }
                        ]
                    },
                    {
                        title:"DC",
                        links:[
                            {
                                url:"#",
                                text:"Terms of Use"
                            },
                            {
                                url:"#",
                                text:"Privacy Policy"
                            },
                            {
                                url:"#",
                                text:"Ad Choices"
                            },
                            {
                                url:"#",
                                text:"Advertising"
                            },
                            {
                                url:"#",
                                text:"Jobs"
                            },
                            {
                                url:"#",
                                text:"Subscriptions"
                            },
                            {
                                url:"#",
                                text:"Talent Workshops"
                            },
                            {
                                url:"#",
                                text:"CPSC Certificates"
                            },
                            {
                                url:"#",
                                text:"Ratings"
                            },
                            {
                                url:"#",
                                text:"Shop Help"
                            },
                            {
                                url:"#",
                                text:"Contact Us"
                            },
                        ]
                    },
                    {
                        title:"SITES",
                        links: [
                            {
                                url:"#",
                                text:"DC"
                            },
                            {
                                url:"#",
                                text:"MAD Magazine"
                            },
                            {
                                url:"#",
                                text:"DC Kids"
                            },
                            {
                                url:"#",
                                text:"DC Universe"
                            },
                            {
                                url:"#",
                                text:"DC Power Visa"
                            },
                        ]
                    }
                ]
            }
        }
    }
</script>

<template>
    <section>
        <div class="container">

            <div class="container-menu">
                <div class="slot-menu" v-for="(element, index) in menu" :key="index">
                    <h4>{{element.title}}</h4>

                    <ul>
                        <li v-for="obj in element.links">
                            <a href="obj.url">
                                {{obj.text}}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="logodc-grande">
                <img src="../assets/images/dc-logo-bg.png" alt="">
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    background-image: url(../assets/images/footer-bg.jpg);
    background-size: cover;
    height: 400px;
    overflow: hidden;

}
.container {
    height: 100%;
    @include between();
}
.container-menu {
    height: 350px;
    padding: 10px;
    @include column();
    gap: 40px;

    h4 {
        margin-bottom: 10px;
    }
    li {
        list-style: none;
    }
    a {
        color: #797979;
        text-decoration: none;
        font-size: 13px;
    }
}
</style>
