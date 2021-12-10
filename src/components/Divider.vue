<template>
  <div class="divider">
    <div class="circle"></div>
    <div class="line"></div>
    <div class="circle"></div>
    <div class="line"></div>
    <div class="circle"></div>
  </div>
</template>

<script>
export default {
  name: "Divider"
}
</script>

<style scoped>
.divider {
  margin-top: 100px;
  width: 20%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.circle {
  width: 50px;
  height: 50px;
  background: #302511;
  border-radius: 50%;
}
.line {
  background: #302511;
  width: 4px;
  height: 350px;
}
</style>