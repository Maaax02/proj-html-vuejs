<template>
  <div class="container">
    <div class="left">
      <ul>
        <li v-for="(item, i) in left" :key="i">
          <i :class="item.class"></i>{{ item.string }}
        </li>
      </ul>
    </div>
    <div class="right">
      <ul>
        <li v-for="(logo, index) in socials" :key="index">
          <i :class="logo"></i>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      left: [
        {
          string: "1.800.567.8910",
          class: "fas fa-phone",
        },

        {
          string: "Contact Us",
          class: "fas fa-envelope",
        },

        {
          string: "Alumni",
          class: "fas fa-graduation-cap",
        },

        {
          string: "Campus",
          class: "fas fa-landmark",
        },
      ],

      socials: {
        ig: "fab fa-instagram",
        twitter: "fab fa-twitter",
        yt: "fab fa-youtube",
        fb: "fab fa-facebook-f",
      },
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/HeaderBox.scss";
</style>