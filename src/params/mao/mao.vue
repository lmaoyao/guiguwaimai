<template>
    <div>
        <Header title="个人中心"></Header>
       <router-link class="login" to="/login" tag="div">
           登录  注册
       </router-link>
    </div>
</template>
<script>
    import Header from "../../components/Header"
    export default {
        components:{
            Header,
        },
    }
</script>
<style lang='stylus' scoped>
    .login
        width 100%
        height 80px
        background aqua
</style>