<template>
  <Nav />
  <Hero />
  <Discover />
  <Contact />
</template>

<script>
import Nav from "./components/Nav";
import Hero from "./components/Hero";
import Discover from "./components/Discover";
import Contact from "./components/Contact";
document.title = "Booked Tool";
export default {
  name: "App",
  components: {
    Nav,
    Hero,
    Discover,
    Contact,
  },
};
</script>
