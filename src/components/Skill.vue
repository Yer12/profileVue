<template>
  <div class="skill d-flex">
    <p class="skill_name">{{ title }}</p>
    <div class="bar">
      <div class="progress" :style="{ 'width': progress + 'px'}">

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skill",
  props: ['title','progress']
}
</script>

<style scoped>
.skill {
  align-items: center;
  display: flex;
  justify-content: space-between;
  padding-right: 50px;
  font-size: 27px;
  margin-bottom: 35px;
}
.skill_name {
  margin: 0;
}
.bar {
  border-radius: 50px;
  background: rgba(149, 157, 157, 0.32);
  width: 180px;
  height: 30px;
}
.progress {
  border-radius: 50px;
  background: rgba(91, 81, 37, 0.43);
  width: 130px;
  height: 30px;
}
</style>