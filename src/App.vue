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
@import url('https://fonts.googleapis.com/css2?family=PT+Sans+Narrow:wght@400;700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');


*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: "PT Sans Narrow", sans-serif;
    font-weight: 900;
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
