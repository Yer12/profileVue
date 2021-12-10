<template>
  <div class="exp_div">
    <h1 class="title">{{experience.direct}}</h1>
    <p class="userspec">{{experience.company}}</p>
    <ul>
      <li v-for="l in experience.doneWorks" v-bind:key="l.id">
        {{l.work}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ExperienceCard",
  props: ['experience']
}
</script>

<style scoped>
.title {
  font-size: 70px;
  color: #302511;
}
.userspec {
  text-transform: uppercase;
  font-size: 30px;
  letter-spacing: 2px;
}
ul {

}
li {
  font-size: 25px;
  width: 100%;
  margin-top: 20px;
  margin-bottom: 0px;
}
</style>