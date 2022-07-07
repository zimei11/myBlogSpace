<template>
  <div class="home">
    <div class="container">
      <div class="card shadow-sm ">
        <div class="card-body">
          <slot></slot>
        </div>
      </div>
    </div>
    <footer>
      <hr class="style1">
      © copyright&nbsp;|&nbsp;Home&nbsp;|&nbsp;zimei
      <div>&nbsp;</div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'ContentBase',
  components: {
  }
}
</script>

<style scoped>
.card {
  margin-top: 20px;
}

/* 页脚 */
footer {
  /* position: fixed;
  bottom: 10px; */
  width: 100%;
  text-align: center;
}

.html,body{
  background-color: aquamarine;
}

/* 水平线 */
hr.style1{
	border-top: 1px solid #8c8b8b;
}
</style>
