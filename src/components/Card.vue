<template>
    
    <div class="card">
        <div><img :src="thumb" alt=""></div>
        <div class="title">{{series}}</div>
    </div>
    
</template>


<script>
export default {
    name: 'Card',
    props: {
        thumb: String,
        series: String,
    },

}
</script>

<style lang="scss" scoped>

    .card {
        width: calc(100% / 6);
        padding: 20px;
        color: white;
        
        .title{
            font-family: 'Roboto', serif;
        }


        img {
            width: 100%;
        }
    }

</style>