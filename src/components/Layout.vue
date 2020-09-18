<template>
    <div class="layout">
        <SideBar />
        <Container />
    </div>
</template>
<script>

import SideBar from "./SideBar"
import Container from "./Container"
export default {
    components:{
        SideBar,
        Container
    }
}
</script>
<style lang="">
    .layout{
        background: rgb(151, 241, 151);
        display: flex;
    }
</style>