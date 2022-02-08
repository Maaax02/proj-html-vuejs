<template>
  <div class="container">
    <main>
      <div class="top">
        <h1>Inspiring Tomorrow Leaders</h1>
      </div>
      <div class="middle">
        <span>The future Belongs To Those Who See Possibilities Today</span>
      </div>
      <div class="buttons">
        <button class="first">FIND A COURSE</button>
        <button class="second">APPLY NOW</button>
      </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  height: 700px;
  background-image: url("../../public/img/home_main_slider_bg.jpg");
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  text-align: center;

  .top {
    font-size: 40px;
    margin-bottom: 20px;
  }

  .middle {
    margin-bottom: 30px;

    span {
      font-size: 25px;
    }
  }

  .buttons{
      width: 270px;
      margin: 0 auto;
      display: flex;
      justify-content: center;
      justify-content: space-around;
      button{
         border: none;
         padding: 10px 15px; 
         color: #fff;
      }

      .first{
          background-color: #FFAB0B;

      }

      .second{
          background-color: #0EBCF2;
      }
  }
}
</style>