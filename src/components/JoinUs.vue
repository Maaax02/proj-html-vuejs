<template>
  <div class="container">
    <div class="text">
      <p>
        Joing Over
        <span
          >500,000 Students
          <div class="line"></div
        ></span>
        Enjoying Avada Education now
      </p>
      <p class="gray">
        Become Part of Avada University to further your Career.
      </p>
    </div>
    <div class="label">
      <input type="text" placeholder="Name" v-model="name" />
      <input type="text" placeholder="Email" v-model="email" />
      <input type="text" placeholder="Telephone" v-model="number" />
      <button @click="openModale()">APPLY NOW</button>
    </div>
    <div class="bg-modale">
      <div class="modal-contents">
        <button class="close" @click="closeModale()">Change Your Infos</button>
        <img src="../../public/img/page-logo-1.png" alt="" />
          <h5>Your information has been saved.</h5>
          <div>
            <ul>
              <li><span>User Name:</span> {{name}}</li>
              <li><span>Email:</span> {{email}}</li>
              <li><span>Telephone:</span> {{number}}</li>
            </ul>
          </div>
        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      number: "",
    };
  },
  methods: {
    openModale() {
      document.querySelector(".bg-modale").style.display = "flex";
    },

    closeModale() {
      document.querySelector(".bg-modale").style.display = "none";
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/JoinUs.scss";
</style>