<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <router-link id='toplogo' class="navbar-brand" :to="{name: 'home'}" >MySpace</router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText"
                aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarText">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link" aria-current="page" href="/">首页</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/userlist">用户列表</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="/userprofile">用户动态</a>
                    </li>
                </ul>
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="/login">登录</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="regist">注册</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default{
    name:"NavBar",
}
</script>

<style scoped>
</style>