<template>
    <ContentBase>
        <div class="alert alert-danger">
            <button type="button" class="close" data-dismiss="alert" aria-hidden="true">◑﹏◐</button>
            <strong>404!</strong> 页面走丢了
        </div>

    </ContentBase>
</template>

<script>
import ContentBase from "../components/ContentBase"

export default {
    name: "NotFoundView",
    components: {
        ContentBase,
    }
}
</script>

<style scoped>
</style>