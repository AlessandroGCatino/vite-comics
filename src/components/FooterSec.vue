<script>
    export default{
        name: "FooterSec",
        data(){
            return{
                footerNavs:[
                    {
                        name: "DC Comics",
                        elements: [
                        "characters",
                        "comics",
                        "movies",
                        "tv",
                        "games",
                        "videos",
                        "news"
                        ]
                    },
                    {
                        name: "shop",
                        elements: [
                        "shop DC",
                        "shop DC collectibles"
                        ]
                    },
                    {
                        name: "dc",
                        elements: [
                        "terms of use",
                        "privacy policy (new)",
                        "ad choices",
                        "advertising",
                        "jobs",
                        "subscriptions",
                        "talent workshops",
                        "CPSC certificates",
                        "ratings",
                        "shop help",
                        "contact us"
                        ]
                    },
                    {
                        name: "sites",
                        elements: [
                        "DC",
                        "MAD magazine",
                        "DC kids",
                        "DC universe",
                        "DC power visa"
                        ]
                    }

                ]
            }
        }
    }
</script>

<template>
    <div id="heroesBack">
        <div class="container">
            <div v-for="(singleRow, index) in footerNavs" :key="index">
                <h3 class="text-uppercase">{{ singleRow.name }}</h3>
                <ul class="d-flex flex-column">
                    <li v-for="(element) in singleRow.elements"
                    class="text-capitalize">
                        {{ element }}
                    </li>
                </ul>
            </div>
            
        </div>

    </div>

</template>

<style scoped>

#heroesBack{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 400px;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white;
}
.container{
    padding-block: 30px;
    height: 400px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 20px;
    align-items: flex-start;
    justify-content: flex-start;
}

ul{
    padding: 0;
    align-items: flex-start;
}


</style>