<template>
  <nav class="navbar-container">
    <div class="navbar-content-container">
      <div class="navbar-content">
        <ul>
          <li v-for="menu in menus" :key="menu.name">{{ menu.name }}</li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavbarDesktop",
  // eslint-disable-next-line vue/require-prop-types
  props: {
    menus: Array,
  },
};
</script>

<style>
.navbar-container {
  display: block;
  width: 100%;
  background: #000;
  background: rgb(146, 146, 146);
}

.navbar-content-container {
  max-width: 800px;
  padding: 12px 24px;
  display: flex;
  justify-content: flex-end;
}
.navbar-content > ul {
  display: flex;
}

.navbar-content > ul > li {
  text-decoration: none;
}
.navbar-content > ul {
  display: flex;
}

@media screen and (max-width: 600px) {
  .navbar-container {
    display: hidden;
  }
}
</style>
