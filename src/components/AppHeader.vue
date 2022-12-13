<script >

    export default{
        name: 'AppHeader',
        data() {
            return {
                argomenti: [
                    {
                        text:"CHARACTERS",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"COMICS",
                        url:"#",
                        current: true,
                    },
                    {
                        text:"MOVIES",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"TV",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"GAMES",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"COLLECTIBLES",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"VIDEOS",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"FANS",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"NEWS",
                        url:"#",
                        current: false,
                    },
                    {
                        text:"SHOP",
                        url:"#",
                        current: false,
                    }
                ]
            }
        }
    }

</script>

<template>

  <header>
    <div class="stacco-sopra"></div>
        <div class="container">

            <div class="logo-section">
                
                <img src="../assets/images/dc-logo.png" alt="DC logo">
                
            </div>
        
            <nav class="nav-section">
                <ul>
                    <li v-for="(link, index) in argomenti" :key="index">
                        <a :class="{active: link.current}" href="#">
                            {{link.text}}
                        </a>
                    </li>
                    
                </ul>
            </nav>

        </div>  
        <div class="stacco-sotto">

        </div>
  </header>


</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
    header {
        text-align: center;
        height: 100px;
    }

    .stacco-sopra, .stacco-sotto {
        width: 100%;
        height: 30px;
        background-color: #1c1c1c;
    }
    .container {
        height: 100%;
        margin-bottom: 20px;
        @include between();
    }

    .logo-section {
        height: 80px;
        width: 100px
    }

    .nav-section {
        height: 100%;

        ul {
            @include center();
            list-style: none;
            margin: 10px 10px ;
            height: 100%;

            li a {
                padding: 10px;
                display: inline-block;
                text-decoration: none;
                transition: background 0.3s;

                &.active,
                &:hover {
                    color: rgb(38, 27, 247);
                    border-bottom: solid 3px rgb(38, 27, 247) ;
                }
            }
        }
    }
    
    
</style>
