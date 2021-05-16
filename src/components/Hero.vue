<template>
  <section class="hero">
    <div class="hero__images">
      <div class="hero__contents">
        <img class="hero__image-1" src="../assets/hero-1.webp" />
        <div class="hero__content">
          <p><strong>Booked Tool</strong> enables you to</p>
          <p>create Interactive Advertisement</p>
          <button>What is it?</button>
        </div>
      </div>
      <img class="hero__image-2" src="../assets/hero-2.webp" />
    </div>
    <LoginForm />
  </section>
</template>

<script>
import LoginForm from "./LoginForm";
export default {
  components: {
    LoginForm,
  },
};
</script>
