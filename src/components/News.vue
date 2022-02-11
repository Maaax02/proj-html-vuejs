<template>
  <div class="container">
    <div class="top">
      <img src="../../public/img/page-logo-1.png" alt="" />
      <h1>Today's University News</h1>
      <span
        >Covering topics from classes to politics and student organization
        events.</span
      >
    </div>
    <div class="line"></div>
    <div class="section">
      <div class="card" v-for="(item, i) in section" :key="i">
        <div class="image" :class="item.image"></div>
      
        <div class="middle">
          <h3>{{ item.title }}</h3>
          <span>{{item.by}} <span id="admin">{{item.author}}</span>{{ item.date }}</span>
        </div>
        <div class="bottom">
          {{ item.read }}
          <i :class="item.class"> 0</i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      section: [
        {
          image: "first",
          title: "What do successful grads think you should study?",
          by : 'By',
          author : ' Admin',
          date: " | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
        {
          image: "second",
          title: "Former student discusses success in the fashion industry",
          by : 'By',
          author: 'Admin',
          date: " | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
        {
          image: "third",
          title: "How do you best prepare for university?",
          by : 'By',
          author : 'Admin',
          date: " | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/News.scss"
</style>