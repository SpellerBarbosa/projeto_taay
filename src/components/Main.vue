<template>
    <div class="main-container">
        <Banner />
        <CardsProdutos />
    </div>
</template>

<script>
import Banner from './MainComponents/Banner.vue';
import CardsProdutos from './MainComponents/CardsProdutos.vue';

export default {
    name:"Main",
    components:{
        Banner,
        CardsProdutos
    }
}
</script>

<style scoped>
    .main-container{
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-items: center;
        align-items: center;
    }
</style>
