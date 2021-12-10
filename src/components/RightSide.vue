<template>
  <div class="rightside">
    <div class="experience">
      <div v-for="e in experiences" v-bind:key="e.id">
        <ExperienceCard :experience="e"/>
      </div>
    </div>
  </div>
</template>

<script>
import ExperienceCard from "./ExperienceCard";
export default {
  name: "RightSide",
  components: {ExperienceCard},
  data() {
    return {
      experiences: [
        {
          id: 1,
          direct: "Frontend",
          company: "Ecomarine | 2019 - 2020",
          doneWorks: [
            {
              id: 1,
              work: "Make some projects in VUE JS",
            },
            {
              id: 2,
              work: "I made a todo list on a VUE with Appolo and GraphQL",
            },

          ]
        },
        {
          id: 2,
          direct: "HTML/CSS developer",
          company: "ONMONDAY | 2020 - 2021",
          doneWorks: [
            {
              id: 1,
              work: "Make some projects in HTML, CSS, JS",
            },
            {
              id: 2,
              work: "I made a todo list on a VUE with Appolo and GraphQL",
            },
            {
              id: 3,
              work: "Made heaps of landings, onilne-magazines",
            },

          ]
        },
        {
          id: 3,
          direct: "Mobilographer",
          company: "BahErs | 2018 - 2019",
          doneWorks: [
            {
              id: 1,
              work: "I am shooting some atmospheric videos on iPhone",
            },
            {
              id: 2,
              work: "And editing(montage) videos",
            },

          ]
        },
      ]
    }
  }
}
</script>

<style scoped>
.rightside {
  width: 40%;
  color: #4d3e22
}

</style>