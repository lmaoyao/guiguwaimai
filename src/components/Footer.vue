<template>
    <div class="foot">
        <div class="guide_item" :class="{on:'/home'===$route.path}" @click="goto('/home')">
    <span class="item_icon">
    <i class="iconfont icon-shouye"></i>
    </span>
            <span>首页</span>
        </div>
        <div class="guide_item" :class="{on:'/list'===$route.path}" @click="goto('/list')">
    <span class="item_icon">
    <i class="iconfont icon-chazhaobiaodanliebiao"></i>
    </span>
            <span>列表页</span>
        </div>
        <div class="guide_item" :class="{on:'/xqy'===$route.path}" @click="goto('/xqy')">
    <span class="item_icon">
    <i class="iconfont icon-shoucang"></i>
    </span>
            <span>收藏</span>
        </div>
        <div class="guide_item" :class="{on:'/mao'===$route.path}" @click="goto('/mao')">
    <span class="item_icon">
    <i class="iconfont icon-wode"></i>
    </span>
            <span>个人中心</span>
        </div>

    </div>
</template>
<script>
    export default {
        methods:{
            goto(path){
                this.$router.push(path)
            }
        }
    }
</script>
<style lang='stylus' scoped>
.foot
    width 100%
    height 60px
    background chocolate
    position fixed
    bottom 0
    left 0
    display flex
    flex-wrap nowrap
    justify-content space-between
    .guide_item
        margin 5px
        color blue
        &.on
            color red
    span
        font-size 12px
        margin-top 2px
        margin-bottom 2px
        .iconfont
            font-size 25px
            display block
</style>