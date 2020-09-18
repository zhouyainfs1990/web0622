<template>
    <div class="main">

        
        <!-- 使用自定义属性向子组件传值 props传值 -->
        <!-- <ListItem 
                    
                    title="学院动态"
                    url="http://www.ujiuye.com/uploadfile/2020/0329/20200329033305219.jpg" :arr="[1,2,3]" /> -->
        
        <!-- = 前面的title 是动态自定义属性， = 后面的是data 里面名称为txt 的数据 -->
        <!-- <ListItem :title="txt"  url="http://www.ujiuye.com/uploadfile/2020/0827/20200827043644872.jpg" /> -->
    
        <ListItem1 v-for="(item,index) in list" :key="index" :item="item"></ListItem1>
    </div>
</template>
<script>
import ListItem from "./ListItem"
import ListItem1 from "./ListItem1"
export default {
    data(){
        return{
            txt:"学员活动",

            list:[{
                title:"学院动态",
                url:"http://www.ujiuye.com/uploadfile/2020/0329/20200329033305219.jpg",
                arr:[1,2,3]
            },{
                title:"学员活动",
                url:"http://www.ujiuye.com/uploadfile/2020/0827/20200827043644872.jpg",
                arr:[4,5,6]
            }]
        }
    },
    components:{
        ListItem,
        ListItem1
    }
}
</script>
<style lang="">
    
</style>