<template>
  <div class="container">
    <div class="image">
      <img src="../../public/img/university_logo.png" alt="" />
    </div>

    <div class="right">
      <ul>
        <li v-for="(item, i) in nav" :key="i">
          <a href="#">{{ item }}</a>
          <drop-down :items="dropDown" />
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import DropDown from "./DropDown.vue";
export default {
  components: { DropDown },
  data() {
    return {
      flag: false,
      nav: [
        "HOME",
        "ABOUT",
        "COURSES",
        "EVENTS",
        "FACILITIES",
        "NEWS",
        "ADMISSIONS",
      ],
      dropDown: [
        {
          title: "Web",
          link: "#",
        },
        {
          title: "Us",
          link: "#",
        },
        {
          title: "University",
          link: "#",
        },
      ],
    };
  },
  methods: {
    open() {
      this.flag = !this.flag;
    },
  },
};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 130px;

  ul {
    list-style: none;
    display: flex;
    align-items: center;

    li {
      margin-left: 60px;
      transition: all 0.8s;

      a {
        text-decoration: none;
        color: black;
        &:hover {
          text-decoration: underline;
          transition: all 0.8s;
          cursor: pointer;
          color: #ffab0b;
        }
      }

      .hidden {
        width: 100px;
        height: 100px;
        background-color: red;
      }
    }
  }
}
</style>