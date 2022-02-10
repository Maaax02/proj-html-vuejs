<template>
  <div class="container">
    <main>
      <div class="left">
        <h1>WORLD CLASS FACILITIES</h1>
        <p>
          Avada university is devoted to exellence in teaching learning and
          research, and developing leaders in many disciplineswho make a
          difference globally
        </p>

        <div class="data">
          <div class="inner" v-for="(item, i) in facilities" :key="i">
            <i :class="item.class"></i>
            <h3>{{ item.title }}</h3>
            <span>- {{ item.text }} </span>
          </div>
        </div>
        <p>
          If you prefer to study in your own time and at your own speed then one
          of our e-learning packages may be right up in your street.
        </p>
      </div>
      <div class="right">
        <h1>OUR VALUES</h1>
        <div class="our-box" v-for="(item, i) in values" :key="i">
          <span>+</span> {{ item }}
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      values: [
        "OUR MISSION",
        "OUR PHILOSOPHY",
        "OUR COMMITMENT",
        "OUR PROMISE",
        "OUR VALUES",
      ],

      facilities: [
        {
          class: "fas fa-globe",
          title: "Internationa Focus",
          text: "our students come from across the globe",
        },
        {
          class: "fas fa-graduation-cap",
          title: "Residential courses",
          text: "we encourage learning and growth",
        },
        {
          class: "far fa-id-badge",
          title: "People not profits",
          text: "education is a right not a privilege",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/ClassFacilities.scss";
</style>