<template>
  <div id="nav">
    <div class="nav_left">
      <img class="logo" src="/logo.png" />
      <router-link class="nav_link" to="/">Pricing & Plans</router-link>
      <router-link class="nav_link" to="/">Contact Us</router-link>
    </div>
    <div class="nav_right">
      <router-link class="login" to="/">Login</router-link>
      <router-link class="signup" to="/signup">Signup</router-link>
    </div>
  </div>
  <router-view />
</template>

<style lang="scss">
#app {
  position: fixed;
  height: 100vh;
  width: 100vw;
  margin: 0;
  padding: 0;
  z-index: 10;
}

#nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 81px;
  margin: 0 auto;
  align-items: center;
}

.nav_left {
  display: flex;
  align-items: center;
  margin-left: 10px;
  height: 100%;
}

.nav_right {
  display: flex;
  align-items: center;
  margin-right: 2rem;
  height: 100%;
}

.nav_link {
  margin-right: 2rem;
  margin-left: 2rem;
}

.logo {
  align-self: center;
  width: 151px;
  height: 28px;
  margin-right: 3rem;
  margin-left: 1rem;
}

.login {
  color: white;
  margin-right: 2rem;
  margin-left: 2rem;
}

.signup {
  display: flex;
  color: white;
  border: 2px solid white;
  align-self: center;
  align-items: center;
  text-align: center;
  justify-content: center;
  height: 50px;
  width: 100px;
  transition: all 0.25s ease-out;
}

.signup:hover {
  background-color: white;
  color: blueviolet;
  transition: all 0.25s ease-out;
}
</style>
