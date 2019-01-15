<template>
    <div class="header">
        <span>
            <span>{{title}}</span>
        </span>
    </div>
</template>
<script>
    export default {
        props:{
            title:String
        }
    }
</script>
<style lang='stylus' scoped>
    .header
        width 100%
        height 30px
        background chocolate
        text-align center
        font-size 20px
</style>