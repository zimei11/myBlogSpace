<template>
    <div class="card  bg-light" >
        <div class="card-body">
            <div v-for="post in posts.posts" :key="post.id">
            <div class="card single-post">
                <dev class="card-body">
                    {{post.content}}
                </dev>
            </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "UserPost",
    props: {
        posts: {
            type: Object,
            required: true,
        }
    },
}
</script>

<style scoped>
.single-post{
    margin-bottom: 10px;
}
</style>