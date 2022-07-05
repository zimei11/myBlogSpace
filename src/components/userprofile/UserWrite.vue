<template>
    <div class="card edit-field">
        <div class="card-body">
            <div class="mb-3">
                <label for="edit-post" class="form-label">编辑帖子</label>
                <textarea class="form-control" id="edit-post" rows="3"></textarea>
                <button type="button" class="btn btn-outline-success btn-sm">发帖</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "UserWrite",
}
</script>

<style scoped>
.edit-field {
    margin-top: 10px;
}

button{
    margin-top: 10px;
}
</style>