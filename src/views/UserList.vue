<template>
    <ContentBase>
        <div class="alert alert-primary" role="alert">
            <strong>用户列表</strong> <a href="https://www.baidu.com" class="alert-link">访问本人博客</a>
        </div>
        <div class="card" v-for="user in users" :key="user.id">
            <div class="card-body">
                <div class="row">
                    <div class="col-1">
                        <img style="height:48px;width: 48px" :src="user.photo" alt="">
                    </div>
                    <div class="col-11">
                        <div class="username">{{user.username}}</div>
                        <div class="follower-count">{{user.followerCount}}</div>
                    </div>
                </div>
            </div>
        </div>
    </ContentBase>
</template>

<script>
import ContentBase from "../components/ContentBase";
import $ from "jquery";
import { ref } from "vue";


export default {
    name:"UserList",
    components:{
        ContentBase,
    },
    setup(){
        let users=ref([]);

        $.ajax({
            url:"https://app165.acapp.acwing.com.cn/myspace/userlist/",
            type:"get",
            success(resp){
                users.value=resp;
            }
        })
        return{
            users,
        }
    }
}
</script>

<style scoped>
img{
    border-radius: 50%;
}

.username{
    font-weight: bold;
    height: 50%;
}

.follower-count{
    font-size: 12px;
    color: gray;
    height: 50%;
}

.card{
    margin-bottom: 20px;
    cursor: pointer;
}

.card:hover{
    box-shadow: 2px 2px 10px lightgrey;
    transition: 300ms;
}
</style>