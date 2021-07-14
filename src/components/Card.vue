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
        font-family: 'arial', serif;
        
        img {
            width: 100%;
            height: 160px ;
            object-fit: cover;
            object-position: top;
        }

        .title {
            text-transform: uppercase;
            font-size: 12px;
            padding-top: 12px;
        }
    }

</style>