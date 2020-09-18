<template>
    <div class="item">
        <h4>{{title}}</h4>
        <div>
            <img :src="url" alt="">
        </div>
        <ul>
            <li v-for="(item,index) in arr" :key="index">{{item}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    // 申明props 属性接收父组件传递的数据
    // props:["title","url","arr"]
    props:{
        // key: 接收的数据名称，
        // value : 检验的数据类型的构造器
        title:String,
        url:String,
        arr:Array,
    }
}
</script>
<style lang="">
    .item{
        width: 400px;
    }
</style>