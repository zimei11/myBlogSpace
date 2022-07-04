<template>
    <ContentBase>
        <div class="row">
            <div class="col-3">
                <UserProfileInfo />
            </div>
            <div class="col-9">
                <UserProfilePost />
            </div>
        </div>
    </ContentBase>
</template>

<script>
import ContentBase from "../components/ContentBase"
import UserProfileInfo from "../components/userprofile/UserInfo"
import UserProfilePost from "../components/userprofile/UserPost"
import { reactive } from "vue"

export default {
    name: "UserProfile",
    components: {
        ContentBase,
        UserProfileInfo,
        UserProfilePost
    },
    setup(){
        const user=reactive({
            username:"lixishi",
            lastname:"Yan",
            firstname:"Xishi",
            followerCount:0,
            is_followed:false,
        });

        return{
            user:user
        }
    }
}
</script>

<style scoped>
</style>