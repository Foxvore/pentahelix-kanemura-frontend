<script setup>
import { onMounted } from "vue";
import Navbar from "@/components/main_view/Navbar.vue";
import Hero from "@/components/main_view/homepage/Hero.vue";
import Kanemura from "@/components/main_view/homepage/Kanemura.vue";
import Rating from "@/components/main_view/homepage/Rating.vue";
import Signature from "@/components/main_view/homepage/Signature.vue";
import Location from "@/components/main_view/homepage/Location.vue";
import Info from "@/components/main_view/homepage/Info.vue";
import Footer from "@/components/main_view/Footer.vue";

onMounted(() => {
  window.scrollTo(0, 0);
});
</script>

<template>
  <Navbar />
  <div id="main" class="w-full min-h-screen bg-[var(--color-cream)] py-20">
    <div id="hero">
      <Hero />
    </div>
    <div id="kanemura">
      <Kanemura />
    </div>
    <div id="rating">
      <Rating />
    </div>
    <div id="signature">
      <Signature />
    </div>
    <div id="location">
      <Location />
    </div>
    <div id="info">
      <Info />
    </div>
  </div>
  <Footer />
</template>
