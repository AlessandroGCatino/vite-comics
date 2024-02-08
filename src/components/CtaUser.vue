<script>
    export default{
        name: "CtaUser",
        data(){
            return{
                ctaElements: [
                    {
                        icon: "src/assets/img/buy-comics-digital-comics.png",
                        text: "digital comics"
                    },
                    {
                        icon: "src/assets/img/buy-comics-merchandise.png",
                        text: "dc merchandise"
                    },
                    {
                        icon: "src/assets/img/buy-comics-subscriptions.png",
                        text: "subscription"
                    },
                    {
                        icon: "src/assets/img/buy-comics-shop-locator.png",
                        text: "comic shop locator"
                    },
                    {
                        icon: "src/assets/img/buy-dc-power-visa.svg",
                        text: "dc power visa"
                    },
                ]
            }
        }
    }
</script>

<template>
    <div id="ctaBack">
        <div class="container">
            <ul class="d-flex gap-5 align-items-center justify-content-center py-4">
                <li v-for="(element, index) in ctaElements" :key="index"
                class="d-flex align-items-center gap-2 p-2">
                    <figure>
                        <img :src="element.icon" alt="" width="45">
                    </figure>
                    <span class="text-uppercase">
                        {{ element.text }}
                    </span>

                </li>
            </ul>
        </div>
    </div>

</template>

<style scoped lang="scss">

@use "../styles/partials/variables.scss" as *;

#ctaBack{
    background-color: $dc-blue;
    color: white;
    font-weight: 500;
}

</style>