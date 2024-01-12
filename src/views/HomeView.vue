<template>
  <div class="home">
    <app-navbar />
    <div class="background">
      <div class="row">
        <div class="col-12 text-center">
          <div class="background-with-text">
            <h1>MAHSYARI OUTFIT</h1>
            <p>
              Where Fashion Meets Comfort, <br />
              Because you deserve to look and feel your best.
            </p>
            <button class="btn btn-primary" @click="toggleLoginForm">Buy Now</button><br /><br />

            <form v-if="showLoginForm" @submit.prevent="submitLoginForm" class="signup-form">
              <div class="form-group">
                <b><label for="email">Email:</label></b>
                <input type="email" v-model="email" class="form-control smaller-input" required />
              </div>
              <div class="form-group"><button type="submit" class="btn btn-primary">Sign Up</button> <button type="button" @click="hideLoginForm" class="btn btn-secondary">Cancel</button></div>
            </form>
          </div>
        </div>
      </div>
    </div>
    <app-footer />
  </div>
</template>

<script>
import AppNavbar from "@/components/AppNavbar.vue";
import AppFooter from "@/components/AppFooter.vue";

export default {
  name: "HomeView",
  components: {
    AppNavbar,
    AppFooter,
  },
  data() {
    return {
      showLoginForm: false,
      email: "",
    };
  },
  methods: {
    submitLoginForm() {
      console.log("Form Submit:", this.email);
      this.hideLoginForm();
    },
    toggleLoginForm() {
      this.showLoginForm = !this.showLoginForm;
    },
    hideLoginForm() {
      this.showLoginForm = false;
    },
  },
};
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
}

.background {
  background-image: url("~@/assets/Images/bg.png");
  width: 100%;
  height: 540px;
  background-size: cover;
  padding: 200px 0 80px;
}

.background-with-text {
  text-align: left;
  margin-top: -130px;
  margin-left: 200px;
}

.smaller-input {
  width: 200px;
  margin-right: 10px;
}

.signup-form {
  display: flex;
  flex-direction: column;
}
.signup-form .form-group {
  margin-bottom: 10px;
}
</style>
