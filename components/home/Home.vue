<script setup>
import Footer from "../layout/Footer.vue";
import Header from "../layout/Header.vue";
import HeroSection from "./HeroSection";
import MarketSection from "./MarketSection.vue";
import AboutSection from "./AboutSection.vue";
import BlogSection from "./BlogSection.vue";
</script>

<template>
  <Header></Header>
  <main>
    <HeroSection />
    <Divider />
    <MarketSection />
    <Divider />
    <AboutSection />
    <Divider />
    <BlogSection />
    <Divider />
    <Footer />
  </main>
</template>
