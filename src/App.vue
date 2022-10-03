<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import NavBar from "./components/Navbar/NavBar.vue";
</script>

<template>
  <!-- <header>
    <img
      alt="Vue logo"
      class="logo"
      src="@/assets/logo.svg"
      width="125"
      height="125"
    />

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->
  <!-- eslint-disable-next-line vue/no-multiple-template-root -->
  <div class="main">
    <NavBar />
    <RouterView />
  </div>
</template>

<style></style>
