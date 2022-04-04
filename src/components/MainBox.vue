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
        <button class="second" @click="openModal()">APPLY NOW</button>
      </div>
    </main>
    <div class="bg-modal">
      <div class="modal-contents">
        <div class="close" @click="closeModal()">+</div>
        <img src="../../public/img/university_logo.png" alt="" />

        <form action="">
          <input type="text" placeholder="Name" />
          <input type="email" placeholder="E-Mail" />
          <a href="#" class="button" @click="closeModal()">Submit</a>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    openModal() {
      document.querySelector(".bg-modal").style.display = "flex";
    },
    closeModal() {
      document.querySelector(".bg-modal").style.display = "none";
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/Main.scss";
</style>