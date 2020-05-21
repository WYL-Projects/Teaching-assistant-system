<template>
    <el-container>
        <el-header height="auto">
            <logo/>
        </el-header>
        <el-main>
            <img src="https://www.jd100.com/static/media/pic_login.63c7ae3b.png" alt="">
            <div class="right">
                <h2>密码登录</h2>
                <el-input
                        placeholder="请输入账号或手机号"
                        v-model="input"
                        clearable>
                </el-input>
                <el-input placeholder="请输入密码" v-model="input1" show-password></el-input>
                <el-button type="primary" @click="login">{{login_btn_info}}</el-button>
            </div>
        </el-main>
    </el-container>
</template>

<script>
    const  logo = ()=> import("../components/logo.vue")
    export default {
        name: "Login",
        components: {
            logo
        },
        data(){
            return {
                input:'',
                input1:'',
                login_btn_info:'登录'
            }
        },
        methods:{
            login(){

            }
        }
    }
</script>

<style scoped>
    .el-header{
        text-align: left;
        background-color: #f7f7f7;
    }
    .el-header>.left{
          justify-content: left;
    }
    .el-main{
        display: flex;
        justify-content: space-around;
    }
    .el-main>img{
    }
    .el-main>.right {
        width: 40%;
        justify-content: right;
    }
    .el-main>.right>.el-input{
        margin-top: 15px;
    }
    .el-main>.right>.el-input>.el-input__inner{
        height: 60px !important;
    }
    .el-main>.right>.el-button{
        width: 100%;
        margin-top: 5px;
    }
</style>