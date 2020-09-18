<template>
    <div class="item">
        <h4>{{item.title}}</h4>
        <div>
            <img :src="item.url" alt="">
        </div>
        <ul>
            <li v-for="(d,index) in item.arr" :key="index">{{d}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    // 申明props 属性接收父组件传递的数据
    // props:["title","url","arr"]
    props:{
       item:Object
    }
}
</script>
<style lang="">
    .item{
        width: 400px;
    }
</style>