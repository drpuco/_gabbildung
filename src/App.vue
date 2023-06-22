<template>
  <Navbar></Navbar>

  <router-view />

  <Footer></Footer>
</template>

<script setup>
  import Navbar from '@/components/Navbar.vue'
  import Footer from '@/components/Footer.vue'
</script>
