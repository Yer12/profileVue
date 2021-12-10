<template>
  <div class="container">
    <Starter/>
    <div style="display: flex; justify-content: space-around">
      <LeftSide />
      <Divider />
      <RightSide />
    </div>
  </div>
</template>

<script>
import RightSide from "./RightSide";
import Divider from "./Divider";
import LeftSide from "./LeftSide";
import Starter from "./Starter";

export default {
  name: "Container",
  components: {
    RightSide,
    Divider,
    LeftSide,
    Starter,
  }
}
</script>

<style scoped>
.container {
  padding-top: 30px;
  background-image: url("../assets/images/header.png");
  background-size: 100%;
  background-repeat: no-repeat;
  padding-left: 230px;
  padding-right: 230px;
  border: 1px solid;
}
</style>