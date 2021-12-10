<template>
  <div class="leftside">
    <div class="education">
      <h1 class="title">Education</h1>
      <p class="userspec">bachelor of design</p>
      <p class="user_univer">Suleyman Demirel University | 2020 - 2024</p>
    </div>

    <div class="skills">
      <h1 class="title">Skills</h1>
      <div v-for="(s,i) in skills" v-bind:key="i">
        <Skill :title="s.title" :progress="s.progress"></Skill>
      </div>
    </div>

    <div class="contact">
      <h1 class="title">Contact</h1>
      <div>
        <div class="contact_div" v-for="c in contacts" v-bind:key="c.id">
          <img :src="c.icon" alt="">
          <p>{{c.text}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Skill from "./Skill";
export default {
  name: "Info",
  components: {Skill},
  data() {
    return {
      skills: [
        {
          id: 1,
          title: "Motion Design",
          progress: 160,
        },
        {
          id: 2,
          title: "Graph Design",
          progress: 110,
        },
        {
          id: 3,
          title: "Illustration",
          progress: 140,
        },
        {
          id: 4,
          title: "Video Editing",
          progress: 60,
        },
      ],
      contacts: [
        {
          id: 1,
          icon: require("../assets/icons/gmail.png"),
          text: "180107136@stu.sdu.edu.kz"
        },
        {
          id: 2,
          icon: require("../assets/icons/phone-call.png"),
          text: "+7(707)523-38-16"
        },
        {
          id: 3,
          icon: require("../assets/icons/location.png"),
          text: "jk Asyl Arman, 2dom, 131kv"
        },
      ]
    }

  },

}
</script>

<style scoped>
.leftside {
  color: #4d3e22;
  width: 40%;
  text-align: left;
}
.education {
  margin-bottom: 100px;
}
.contact {

}
.contact_div {
  display: flex;
  font-size: 25px;
  align-items: center;
  font-weight: bolder;

}
.contact_div img {
  width: 30px;
  height: 30px;
  margin-right: 20px;
}
.title {
  font-size: 70px;
  color: #302511;

}
.userspec {
  text-transform: uppercase;
  font-size: 30px;
  letter-spacing: 2px;
}
.user_univer {
  font-size: 30px;
}


</style>