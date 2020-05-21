<template>
    <div class="left">
        <img class="logo" src="../assets/logo.png" title="轻松学习"/>
        <span class="nettitle">轻松学习网</span>
    </div>
</template>

<script>
    export default {
        name: "logo"
    }
</script>

<style scoped>
    .left{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .logo{
        width: 150px;
        height: 150px;
    }
    .nettitle{
        font-family:KaiTi;
        font-size: 22px;
        font-weight: bold;
    }
</style>