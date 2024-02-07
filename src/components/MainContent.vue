<script>

    import CtaUser from "./CtaUser.vue"

    export default{
        name: "MainContent",
        components: {
            CtaUser
        }
    }


</script>

<template>

    <div class="back">
        <div class="container p-5">
            <h2 class="text-uppercase"> --> content goes here &lt;-- </h2>
        </div>
    </div>
    <CtaUser/>

</template>

<style scoped>

div.back{
    background-color: #1c1c1c;
}

h2{
    color: white;
}

</style>