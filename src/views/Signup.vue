<template>
  <div class="container">
    <div class="form"></div>
    <div class="image">
      <h2 class="header_2">Better, Faster, Secure</h2>
      <div class="description">Start accepting payments with Money Space</div>
    </div>
  </div>
</template>

<script lang="ts"></script>

<style lang="scss">
.container {
  display: flex;
  position: absolute;
  top: 0;
  width: 100vw;
  height: 100vh;
  z-index: -1;
}
.form {
  width: 50%;
  height: 100%;
}
.image {
  width: 50%;
  height: 100%;
  background-image: url("/img01.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
