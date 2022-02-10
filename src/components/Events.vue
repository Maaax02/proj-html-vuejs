<template>
  <div class="container">
    <div v-for="(item, i) in here" :key="i" :class="item.class">
      <h2>{{ item.title }}</h2>
      <div class="line"></div>
      <span>{{ item.text }}</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      here: [
        {
          class: "left",
          title: "COURSES",
          text: "View More",
        },
        {
          class: "middle",
          title: "EVENTS",
          text: "View More",
        },
        {
          class: "right",
          title: "LATEST NEWS",
          text: "View More",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/Events.scss";
</style>