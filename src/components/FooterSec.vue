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

                ],
                socials: [
                    {
                        name:"facebook",
                        source: "src/assets/img/footer-facebook.png"
                    },
                    {
                        name:"twitter",
                        source: "src/assets/img/footer-twitter.png"
                    },
                    {
                        name:"youtube",
                        source: "src/assets/img/footer-youtube.png"
                    },
                    {
                        name:"pinterest",
                        source: "src/assets/img/footer-pinterest.png"
                    },
                    {
                        name:"periscope",
                        source: "src/assets/img/footer-periscope.png"
                    }
                ]
            }
        }
    }
</script>

<template>
    <div id="heroesBack">
        <div class="container">
            <div class="left-column col-4">
                <div v-for="(singleRow, index) in footerNavs" :key="index">
                    <h3 class="text-uppercase">{{ singleRow.name }}</h3>
                    <ul class="d-flex flex-column">
                        <li v-for="(element) in singleRow.elements"
                        class="text-capitalize">
                            <a href="#"> {{ element }} </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="right-column col-6">
                <figure>
                </figure>
                
            </div>
        </div>
    </div>
    <div class="social">
        <div class="container">
            <div class="d-flex col-3">
                <a href="#" class="text-uppercase"> sign-up now!</a>
            </div>
            <div class="d-flex gap-3">
                <h3 class="text-uppercase">follow us</h3>
                <figure v-for="(element) in socials">
                    <img :src="element.source" :alt="element.name">
                </figure>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

@use "../styles/partials/variables.scss" as *;

#heroesBack{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 400px;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white;
}
.left-column{
    padding-block: 30px;
    height: 400px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 20px;
    align-items: flex-start;
    justify-content: flex-start;
    ul{
        padding: 0;
        align-items: flex-start;
        color: grey;
        li{
            &:hover{
                color: white
        };
        };
    }
}

.container{
    display: flex;
    justify-content: space-between;
}
.social .container{
    align-items: center;
    h3{
        color: $dc-blue;
        font-weight: 700;
        letter-spacing: .1rem;
    }
}

.right-column{
    height: 400px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-position: center;
    background-repeat: no-repeat;
    overflow: hidden;
}

.social{
    background-color: #303030;
    padding: 30px;
    align-items: center;
    justify-content: space-between;
    a{
        border: 2px solid $dc-blue;
        letter-spacing: .2rem;
        font-size: 20px;
        padding: 15px;
        color: white;
    };
    
}


</style>