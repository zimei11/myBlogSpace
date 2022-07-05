<template>
    <ContentBase>
        <div class="alert alert-primary" role="alert">
            <strong>好友列表</strong> <a href="https://www.baidu.com" class="alert-link">访问本人博客</a>
        </div>
    </ContentBase>
</template>

<script>
import ContentBase from "../components/ContentBase";
// import $ from 'jquery';


export default {
    name: "UserList",
    components: {
        ContentBase,
    },
    setup(){

    }
}
</script>

<style scoped>
</style>