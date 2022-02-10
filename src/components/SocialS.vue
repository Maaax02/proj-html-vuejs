<template>
  <div class="container">
    <div>
      <span v-for="(item, i) in datas" :key="i">
        {{ item }}
      </span>
    </div>
    <div class="social">
      <i v-for="(logo, x) in logos" :key="x" :class="logo"> </i>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      datas: [
        " © Theme Fusion | ",
        " All Rights Reserved |",
        " Powered By Wordpress |",
        " Support@theme-fusion.com |",
        " 1.800.555.6789",
      ],
      logos: [
        "fab fa-facebook-f",
        "fab fa-twitter",
        "fab fa-youtube",
        "fab fa-instagram",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: space-between;

  span {
    padding: 0 20px;
  }

  i {
    color: #94979f;
    padding: 0 10px;
    transition: all 1s;
    cursor: pointer;

    &:hover{
      color: #ffab0b;
      transition:all 1s;
    }
  }
  .social {
    margin-right: 150px;
  }
}
</style>