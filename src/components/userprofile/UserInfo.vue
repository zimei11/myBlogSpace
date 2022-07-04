<template>
    <div class="card">
        <div class="card-body">
            <div class="row">
                <div class="col-3">
                    <img width="45px"
                        src="https://cdn.acwing.com/media/user/profile/photo/113094_lg_db881120f8.jpg" alt="">
                </div>
                <div class="col-9">
                    <div class="username">Xishi Li</div>
                    <div class="fans">粉丝数：123</div>
                    <button type="button" class="btn btn-success btn-sm">+关注</button>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: "UserProfileInfo",
}
</script>

<style scoped>
img {
    border-radius: 50%;
}

.username {
    font-weight: bold;
}

.fans {
    font-size: 14px;
    color: gray;
}

button {
    padding: 2px 4px;
    font-size: 12px;
}
</style>