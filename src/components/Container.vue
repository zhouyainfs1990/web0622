<template>
    <div class="container">
        <NavHeader/>
        <v-main></v-main>
    </div>
</template>
<script>
import NavHeader from "./NavHeader"
import Main from "./Main"
export default {
    components:{
        NavHeader,
        "v-main":Main
    }
}
</script>
<style lang="">
    .container{
        flex-grow: 1;
    }
</style>