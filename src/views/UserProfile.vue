<template>
    <ContentBase>
        <div class="row">
            <div class="col-3">
                <UserProfileInfo @follow="follow" @unfollow="unfollow" :user="user" />
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
    setup() {
        const user = reactive({
            userName: "lixishi",
            lastName: "Li",
            firstName: "Xishi",
            followerCount: 0,
            is_followed: false,
        });

        const follow = () => {
            if (user.is_followed) return;
            user.is_followed = true;
            user.followerCount++;
        };
        const unfollow = () => {
            if (!user.is_followed) return;
            user.is_followed = false;
            user.followerCount--;
        }

        return {
            user,
            follow,
            unfollow,
        }
    }
}
</script>

<style scoped>
</style>