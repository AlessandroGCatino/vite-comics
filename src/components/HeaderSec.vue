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

    <div id="external">
        <div class="container py-3 d-flex justify-content-between">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="Header Logo" width="70">
            </figure>
            <nav class="d-flex align-items-center">
                <ul class="d-flex gap-3 text-uppercase">
                    <li v-for= "(elements, index) in navElements" :key="index">
                        <a :href="elements.link"> {{ elements.name }} </a>
                    </li>
                </ul>
            </nav>
        </div>

    </div>

</template>

<style scoped lang="scss">

@use "../styles/partials/variables.scss" as *;

li{
    position: relative;
    &:hover{
        color: $dc-blue;
    }
}

li:hover:after{
    position: absolute;
    content: "";
    width: 100%;
    left: 0;
    bottom: -40px;
    border-bottom: 3px solid $dc-blue;
}

</style>