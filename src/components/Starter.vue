<template>
  <div class="starter d-flex">
    <div class="profile">
      <img class="img" src="../assets/images/me.png">
    </div>
    <div class="user_info">
      <h1 class="username">Eleanor <br>Fitzergald</h1>
      <p class="user_spec">Frontend Developer</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Starter"
}
</script>

<style scoped>
.starter {
  width: 100%;
  justify-content: space-between;
  padding-top: 100px;
  padding-bottom: 100px;
}
.profile {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 600px;
  height: 600px;
  background: #E4E0CA;
  border-radius: 50px;
}
.img {
  width: 540px;
  object-fit: cover;
  height: 540px;
  border-radius: 40px;
  background: #2c3e50;
}
.user_info {
  padding-right: 100px;
}
.username {
  font-size: 120px;
  font-weight: bolder;
  text-align: left;
  margin: 0;
  padding: 0;
  color: #FFF8DE;
}
.user_spec {
  font-size: 50px;
  text-transform: uppercase;
  padding: 0;
  margin: 50px 0 0;
  color: #FFF8DE;
}
</style>