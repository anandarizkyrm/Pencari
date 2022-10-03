<template>
  <section>
    <NavbarDesktop :menus="menus" />
  </section>
</template>

<script>
import NavbarDesktop from "./NavbarDesktop.vue";
export default {
  name: "NavBar",
  components: {
    NavbarDesktop,
  },

  data() {
    return {
      menus: [
        {
          name: "Cmail",
          link: "/",
        },
        {
          name: "Gambar",
          link: "/",
        },
      ],
    };
  },
};
</script>

<style></style>
