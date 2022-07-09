<template>
    <ContentBase>
        <div class="row justify-content-md-center">
            <div class="col-lg-3">
                <form @submit.prevent="login">
                    <div class="mb-3">
                        <label for="username" class="form-label">用户名</label>
                        <input v-model="username" type="text" class="form-control" id="username">
                    </div>
                    <div class="mb-3">
                        <label for="password" class="form-label">密码</label>
                        <input v-model="password" type="password" class="form-control" id="password">
                    </div>
                    <div class="error-message">{{error_message}}</div>
                    <button type="submit" class="btn btn-success">登录</button>
                </form>

            </div>
        </div>


    </ContentBase>
</template>

<script>
import { ref } from "vue";
import ContentBase from "../components/ContentBase";

export default {
    name: "LogInView",
    components: {
        ContentBase,
    },
    setup() {
        let username = ref("");
        let password = ref("");
        let error_message=ref("");

        const login=()=>{
            console.log(username.value,password.value);
        }

        return {
            username,
            password,
            error_message,
            login,
        }
    }
}
</script>

<style scoped>
button{
    width: 100%;
}

.error-message{
    color: red;
}
</style>