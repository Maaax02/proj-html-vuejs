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
          <span>{{ item.date }}</span>
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
          date: "By `<span>admin</span>` | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
        {
          image: "second",
          title: "former student discusses success in the faschion industry",
          date: "By `<span>admin</span>` | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
        {
          image: "third",
          title: "How do you best prepare for university?",
          date: "By `<span>admin</span>` | March 16th, 2016",
          read: "Read More >",
          class: "fas fa-comments",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  .top {
    margin: 60px auto;
    width: 600px;
    text-align: center;
  }
  image {
    margin-top: 140px;
  }

  h1 {
    margin-top: 30px;
    margin-bottom: 15px;
  }

  .line {
    border-bottom: 1px solid #ffab0b;
    width: 200px;
    margin: 20px auto;
  }

  .section {
    display: flex;
    width: 1200px;
    margin: 0 auto;
    justify-content: space-around;
    text-align: left;

    .first{
      background: url("../../public/img/news_single_post_header_1.jpg");
      background-size: cover;
    }

    .second{
      background: url("../../public/img/news_single_post_header_2.jpg");
      background-size: cover;
    }

    .third{
      background: url("../../public/img/news_single_post_header_3.jpg");
      background-size: cover;
    }
    .card {
      height: 400px;
      width: 300px;
      display: flex;
      flex-direction: column;

      .image {
        width: 300px;
        height: 170px;
        margin-bottom: 20px;
      }
      .bottom{
        display: flex;
        justify-content: space-between;
        margin-top: 40px;
        padding: 0 4px;

        i{
          color: #ffab0b;
        }
      }

      .middle{

        h3{
          margin-bottom: 10px;
          color: #ffab0b;
        }
        span{
          font-size: 14px;
          color: #94979f;
        }
      }
    }

  }
}
</style>