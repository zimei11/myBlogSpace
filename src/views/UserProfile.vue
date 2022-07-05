<template>
    <ContentBase>
        <div class="row">
            <div class="col-3">
                <UserProfileInfo @follow="follow" @unfollow="unfollow" :user="user" />
                <UserWrite />
            </div>
            <div class="col-9">
                <UserProfilePost :posts="posts" />
            </div>
        </div>
    </ContentBase>
</template>

<script>
import ContentBase from "../components/ContentBase"
import UserProfileInfo from "../components/userprofile/UserInfo"
import UserProfilePost from "../components/userprofile/UserPost"
import UserWrite from "@/components/userprofile/UserWrite"
import { reactive } from "vue"

export default {
    name: "UserProfile",
    components: {
        ContentBase,
        UserProfileInfo,
        UserProfilePost,
        UserWrite,
    },
    setup() {
        // 用户信息
        const user = reactive({
            userName: "lixishi",
            lastName: "Li",
            firstName: "Xishi",
            followerCount: 0,
            is_followed: false,
        });

        // 帖子
        const posts = reactive({
            count: 3,
            posts: [
                {
                    id: 1,
                    userId: 1,
                    content: "今天上了web课真开心",
                },
                {
                    id: 2,
                    userId: 1,
                    content: "今天上了算法课更开心了",
                },
                {
                    id: 3,
                    userId: 1,
                    content: "今天上了acwing，开心极了!",
                },
            ]
        })

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
            posts,
        }
    }
}
</script>

<style scoped>
</style>