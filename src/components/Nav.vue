<template>
  <nav>
    <button id="notification">
      <img src="../assets/megaphone.svg" alt="notification" class="icon" />
    </button>
    <ul ref="navbar">
      <li class="active">Home</li>
      <li>Discover</li>
      <li>Register</li>
      <li><img src="../assets/search.svg" alt="search" class="icon" /></li>
    </ul>
  </nav>
</template>

<script>
export default {
  methods: {
    handleResponsiveNav() {
      this.$refs.navbar.classList.toggle("responsive");
    },
  },
};
</script>
