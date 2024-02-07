<script>
    export default{
        name: "HeaderSec",
    

        data() {
            return {
                navElements : [
                    {
                        name: "characters",
                        link: "#"
                    },
                    {
                        name: "comics",
                        link: "#"
                    },
                    {
                        name: "movies",
                        link: "#"
                    },
                    {
                        name: "tv",
                        link: "#"
                    },
                    {
                        name: "games",
                        link: "#"
                    },
                    {
                        name: "collectibles",
                        link: "#"
                    },
                    {
                        name: "videos",
                        link: "#"
                    },
                    {
                        name: "fans",
                        link: "#"
                    },
                    {
                        name: "news",
                        link: "#"
                    },
                    {
                        name: "shop",
                        link: "#"
                    }
                ]
            }
        }
    }
</script>

<template>

    <div class="container">
        <figure>
            <img src="../assets/img/dc-logo.png" alt="Header Logo" width="50">
        </figure>

    </div>

</template>

<style>

    .container{
        background-color: red;
    }

</style>