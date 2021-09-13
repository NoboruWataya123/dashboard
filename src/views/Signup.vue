<template>
  <div class="container">
    <div class="form">
      <div class="form-group">
        <h3 class="header_3" for="email">Signup</h3>
        <input
          type="email"
          class="form-control"
          id="email"
          v-model="email"
          placeholder="Email"
        />
        <input
          type="tel"
          class="form-control"
          id="tel"
          v-model="tel"
          placeholder="+"
        />
        <input
          type="password"
          class="form-control"
          id="password"
          v-model="password"
          placeholder="Password"
        />
        <input
          type="password"
          class="form-control"
          id="password"
          v-model="password"
          placeholder="Re-enter Password"
        />
        <input
          type="text"
          class="form-control"
          id="promo"
          v-model="promo"
          placeholder="Promo Code"
        />
        <button class="btn" @click="register" :disabled="loading">
          Register
        </button>
      </div>
    </div>
    <div class="image">
      <div class="hero_text">
        <h2 class="header_2">Better, Faster, Secure</h2>
        <div class="description">Start accepting payments with Money Space</div>
      </div>
    </div>
  </div>
</template>

<script lang="ts"></script>

<style lang="scss" scoped>
.container {
  display: flex;
  position: absolute;
  top: 0;
  width: 100vw;
  height: 100vh;
  z-index: -1;
}

.form {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 50%;
  height: 100vh;
  margin: 6rem 0 0 0;
}

.form-group {
  display: flex;
  width: 60%;
  min-height: 100%;
  flex-direction: column;
}

.header_3 {
  font-size: 41px;
}

.form-control {
  width: 100%;
  height: 55px;
  font-size: 1.2rem;
  padding-left: 1rem;
  margin: 0 0 1.5rem 0;
  border: 2px solid #e3e3e3;
  background-color: #fafafb;
  color: #182e54;
  border-radius: 5px;
  transition: all 0.25s ease-out;
}

.form-control:focus {
  outline: none;
  border: #0d6efd solid 2px;
  border-radius: 5px;
  transition: all 0.25s ease-out;
}

.image {
  width: 50%;
  height: 100%;
  position: fixed;
  top: 0;
  right: 0;
  background-image: url("/img01.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}

.hero_text {
  position: absolute;
  top: 60%;
  left: 0%;
  margin-left: 4rem;
  padding-right: 15%;
}

.header_2 {
  font-size: 4.5rem;
  font-weight: bold;
  color: #fff;
  margin: 0;
}

.description {
  font-size: 1rem;
  color: #fff;
}

.btn {
  width: 104%;
  background: hsl(216, 98%, 52%);
  color: #fff;
  padding: 2px;
  font-size: 1.2rem;
  font-weight: 500;
  height: 55px;
  margin: 0 0 1.5rem 0;
  border: transparent;
  border-radius: 5px;
  cursor: pointer;
  transition: all 0.25s ease-out;
}

.btn:hover {
  background: hsl(216, 98%, 42%);
  transition: all 0.25s ease-out;
}
</style>
