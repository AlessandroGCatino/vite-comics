<template>

    <div>
        <figure>
            <img :src="thumbnail" :alt="series">
        </figure>
        <span> {{ series }} </span>
    </div>

</template>

<script>
    export default{
        name: "SquareCard",
        props:{
            thumbnail: String,
            series: String
        }
    }

</script>

<style scoped lang="scss">

div{
    width: calc(100%/6);
    padding: 20px;

    span{
        color: white;
        font-size: 14px;
        text-transform: uppercase;
    }

    figure{
        width: 100%;
        aspect-ratio: 1;
        overflow: hidden;
        img{
            width: 100%;
            
            display: block;
        }
    }
}
</style>