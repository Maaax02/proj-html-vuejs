<template>
  <div class="menu-item" @click="flag = !flag">
    <i class="fas fa-caret-down"></i>
    <transition class="fade" appear="">
      <div class="sub-menu" v-if="flag">
        <div v-for="(item, i) in items" :key="i">
          <a href="#">{{ item.title }}</a>
        </div>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  props: {
    items: Array,
  },
  data() {
    return {
      flag: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.menu-item {
  display: flex;
  justify-content: center;

  i {
    color: #ffab0b;
    
  }

  i:active > .sub-menu {
      transition: all 1s ease-out;
      color: black;
      background-color: red;
    }

  .sub-menu {
    width: 100px;
    margin: 20px 0;
    text-align: center;
    background-color: #ffab0b;
    height: max-content;
    padding: 8px 10px;
    position: absolute;
    border-radius: 10px;

   

    a {
      text-decoration: none;
      color: #fff;

      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>