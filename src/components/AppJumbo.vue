<script>
export default{
    name:"AppJumbo",
    data() {
        return{
            
        }
    }
}
</script>

<template>
 <section>
    <img src="../assets/images/jumbotron.jpg" alt="">
    
 </section>
</template>

<style lang="scss" scoped>

section {
    height: 400px;

    img{
        height: 100%;
        width: 100%;
        object-fit: cover;
        object-position: 20% 0;
    }
}
</style>
