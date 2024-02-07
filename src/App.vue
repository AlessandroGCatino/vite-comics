<template>

    <HeaderSec/>
    <MainContent/>
    <FooterSec/>


</template>

<script>

    import HeaderSec from "./components/HeaderSec.vue"
    import MainContent from "./components/MainContent.vue"
    import FooterSec from "./components/FooterSec.vue"

    export default{
        components : {
            HeaderSec,
            MainContent,
            FooterSec
        }
    }

</script>


<style lang="scss">

@use "./styles/general.scss";

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

figure{
    margin: 0;
}

li{
    list-style-type: none;
}

a{
    color: inherit;
    text-decoration: none;
}

</style>
