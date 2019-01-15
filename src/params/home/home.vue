<template>
    <div class="home">
        <Header title="毛旺旺的作品"></Header>
        <div class="swiper-container">
            <div class="swiper-wrapper">
                <div class="swiper-slide"><img class="tp" src="./imgs/1.jpg" alt=""></div>
                <div class="swiper-slide"><img class="tp" src="./imgs/4.jpg" alt=""></div>
                <div class="swiper-slide"><img class="tp" src="./imgs/9.jpg" alt=""></div>
            </div>
            <!-- 如果需要分页器 -->
            <div class="swiper-pagination"></div>

            <!-- 如果需要导航按钮 -->
            <div class="swiper-button-prev"></div>
            <div class="swiper-button-next"></div>
            <!-- 如果需要滚动条 -->
            <div class="swiper-scrollbar"></div>
        </div>
    </div>
</template>
<script>
    import Header from "../../components/Header"
    import swiper from "swiper"
    import "swiper/dist/css/swiper.css"
    export default {
        components:{
            Header,
        },
        mounted(){
            //创建一个swiper对象
            new swiper('.swiper-container',{
                loop:true,//循环轮播
                //如果需要分页器
                pagination:{
                    el:".swiper-pagination"
                }
            })
        }
    }
</script>
<style lang="stylus" scoped>
   .home
        background greenyellow
       .swiper-container
            width 100%
            height 100px
            .tp
                width 100%
                height 100%


</style>