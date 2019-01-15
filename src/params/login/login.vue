<template>
    <div class="container">
        <h1 class="iconfont icon-fanhui" @click="$router.back()"></h1>
        <!-- 主体内容 （登陆界面）-->
        <div class="main">
            <!-- 右侧登陆界面 -->
            <div class="sideright">
                <div class="index">
                    <form action="#" method="get">
                        <p class="headline">用户登陆</p>
                        <p class="astyle">用户名：</p>
                        <input type="text" placeholder="请输入您的手机号">
                        <p class="astyle">密码：</p>
                        <input type="text" placeholder="请输入密码">
                        <input type="submit" value="登陆" name="login" >
                        <br>
                        <p class="bstyle"><input type="checkbox" name="rempas" />记住密码</p>
                        <p class="cstyle">忘记密码</p>
                        <br><br>
                        <p class="cstyle">没有账号？<a href="zhuce.html">立即注册</a></p>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    export default {}
</script>
<style>

    .container{
        width: 1200px;
        height: 870px;
        margin: 0 auto;
        /* 	background: #ccc; */
    }
    /* 主题内容 */
    .main{
        width:1200px;
        height: 450px;
    }
    .sideleft{
        width:460px;
        height: 250px;
        float: left;
        padding:85px 130px
    }
    .sideleft p{
        padding: 8px 0;
        font-size: 16px;
    }
    .sideright{
        width: 480px;
        height: 450px;
        float: right;
    }
    .sideright .index{
        width: 330px;
        height: 350px;
        background-color:rgba(255,255,255,0.75);
        margin: 50px 90px;
    }
    .headline{
        font-size: 22px;
        text-align: center;
        padding: 20px;
    }
    input[type="text"],
    input[type="submit"]{
        -web-kit-appearance:none;
        -moz-appearance: none;
        display: block;
        margin: 0 auto;
        font-size:15px;
        width: 240px;
    }
    input[type="text"]{
        height:35px;
        border-radius:3px;
        border:1px solid #c8cccf;
        color:#6a6f77;
        outline:0;
    }
    input[type="submit"]{
        margin-top: 25px;
        height: 35px;
        background: #357eb8;
        color: #bcedff;
        font-weight: bold;
        font-size: 16px;
    }
    input[type="submit"]:hover{
        background: #0e62a3;
        cursor: pointer;
    }
    .astyle{
        margin: 5px 0 5px 42px;
        font-size:17px;
        color: #6a6f77;
    }
    .bstyle{
        display: block;
        float: left;
        margin-left: 46px;
        font-size: 15px;
    }
    .cstyle{
        display: block;
        float: right;
        margin-right: 46px;
        font-size: 15px;
    }
    .cstyle a{
        text-decoration: none;
    }

</style>